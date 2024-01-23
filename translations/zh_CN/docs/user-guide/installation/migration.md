# 升级到 TrombLoader 2

本指南向您展示如何从手动模组安装升级到 r2modman！

!> 请务必仔细阅读本指南以防止出现存档丢失的情况。

## 卸载 TrombLoader 1

TrombLoader 2 更改了处理数据的方式且已经不兼容TrombLoader 1。 在升级时，数据会自动继承，但来回切换有可能会导致存档中的分数记录丢失。

所以本指南会教你如何卸载TrombLoader 1。

1. 打开Steam并右键点击Trombone Champ。 在右键菜单中选择 `管理 > 浏览本地文件`。

![右键菜单预览](../docs/files/localfilescontext.png)

2. 找到 BepInEx 文件夹。
3. 删除 `Plugins` 文件夹。 您将在下一步中使用 r2modman 重新安装您的所有模组。

![插件目录](../docs/files/r2modman-install/deleteplugins.png)

保持此文件夹窗口打开，下面的步骤将会需要该窗口来移动您的 CustomSongs 文件夹！

!> 确保你删除的**不是** `TromboneChamp_Data/Plugins`! 这会导致你的游戏文件损坏。 不过，您可以通过在Steam中验证文件完整性来修复它。

## 安装 TrombLoader 2

请参阅 [安装 r2modman](installing-r2modman)，操作完成后再回到这里！

如果你有其他模组，请使用 r2modman 来重新安装它们！

## 迁移歌曲文件

r2modman将模组文件存储在游戏文件夹之外的“配置文件”目录中。 这意味着它不会加载您现有的自制歌曲，直到您将他们移动到新的位置！

1. 您可以通过点击 r2modman 的“Setteings”->“Browse profile folder”

![Browse profile folder](../docs/files/r2modman-install/browseprofile.png)

2. 找到 BepInEx 文件夹。

![Profile Folder](../docs/files/r2modman-install/profilefolder.png)

3. 移动您旧的 CustomSongs 文件夹到此目录。

![BeepInEx 文件夹](../docs/files/r2modman-install/bepinexfolder.png)
