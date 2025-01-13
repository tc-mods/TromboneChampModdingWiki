# 编写模组

手痒想写自己的模组了是吧！ 往下看！（译者能力有限，推荐直接啃英文。应该不会有人都到这一步了还表示自己看不懂英文吧，不会吧不会吧。）

?> 除了这篇指南以外您也可以读一读BepInEx的[广泛适用的入门指南](https://docs.bepinex.dev/articles/dev_guide/plugin_tutorial/index.html)！

## 创建项目

您的编辑器可能有一个“创建项目”按钮。 [Rider](https://jetbrains.com/rider/)的界面看起来就像这样：

![Rider 'new solution' page](../docs/files/new_solution.png)

您想选择 "Class Library" 作为项目类型。 正确的目标框架是 **.NET 4.7.2**, 尽管runtime实际是 Unity Mono, 且有一些问题。 如果您不能选择 `net472`, 请选择 `netstandard 2.1` 并在 `.csproj` 中手动更改它。

### NuGet note

BepInEx 将他们的软件包托管在他们自己的Nuget 服务器上，所以一旦你设置了这个项目，你将需要添加一个`NuGet.config` 在你的solution file文件中，包含以下内容：

```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
    <packageSources>
        <add key="BepInEx" value="https://nuget.bepinex.dev/v3/index.json" />
    </packageSources>
</configuration>
```

## 设置您的 `.csproj`

生成的 `.csproj` 现在看起来很可能是空的：

```xml
<!-- The `Sdk` property automatically sets up a lot of things for us (i.e. standard library!) -->
<Project Sdk="Microsoft.NET.Sdk">

    <PropertyGroup>
        <!-- Change this to net472 if you created it as netstandard2.1 -->
        <TargetFramework>net472</TargetFramework>
        <Nullable>enable</Nullable>
    </PropertyGroup>

</Project>
```

既然您正在为 Trombone Champ开发模组，您将需要实际游戏代码！ 幸运的是，我们已将代码上传至NuGet上，所以你可以简单地将下面的内容添加到你的 `.csproj`文件中。在 `</PropertyGroup>`末尾的下方:

```xml
<ItemGroup>
    <!-- Required: BepInEx and the game code itself! -->
    <PackageReference Include="BepInEx.Core" Version="5.*" />
    <PackageReference Include="TromboneChamp.GameLibs" Version="%{nuget:TromboneChamp.GameLibs:highlighted}" />

    <!-- BaboonAPI provides useful hooks and patches for mods, -->
    <!-- but it's not strictly required -->
    <PackageReference Include="TromboneChamp.BaboonAPI" Version="%{nuget:TromboneChamp.BaboonAPI:highlighted}" />
</ItemGroup>
```

### 调用TrombLoader

TrombLoader 现在也在 Nuget 上，因此你可以直接添加一个软件包引用：

```xml
<PackageReference Include="TromboneChamp.TrombLoader" Version="%{nuget:TromboneChamp.TrombLoader:highlighted}" />
```

## 基本设置

现在您已经准备完毕了，可以开始编写您的插件了！ 您的主要入口点是扩展了 `基础插件的` 类：

```csharp
[BepInPlugin("ch.offbeatwit.chimpanzee", "Chimpanzee", "1.0.0.0")]
public class ChimpanzeePlugin : BaseUnityPlugin
{
```

`BaseUnityPlugin` 实际上只是一种特殊的MonoBehaviour。 所以你可以实现任何基本的 Unity 事件功能 ！ 您的初始设置应该都在Awake中。

```csharp
    private void Awake()
    {
        // Setup goes here!
    }
}
```

## 使用 BaboonAPI 的基本设置

[BaboonAPI](https://baboonapi.trombone.wiki/)提供了一个"安全启动" API, 有助于在游戏出现任何错误时安全的停止游戏的加载。

首先，如果您想要添加 BaboonAPI 作为一个BepInDependency：

```csharp
using BaboonAPI.Hooks.Initializer;

[BepInPlugin("ch.offbeatwit.chimpanzee", "Chimpanzee", "1.0.0.0")]
[BepInDependency("ch.offbeatwit.baboonapi.plugin")]
public class ChimpanzeePlugin : BaseUnityPlugin
{
```

然后你可以使用 GameInitializationEvent：

```csharp
    private Harmony _harmony = new Harmony("ch.offbeatwit.chimpanzee");

    private void Awake()
    {
        GameInitializationEvent.Register(Info, TryInitialize);
    }

    private void TryInitialize()
    {
        // Harmony patches can fail to apply, so do them here
        _harmony.PatchAll();
    }
}
```
