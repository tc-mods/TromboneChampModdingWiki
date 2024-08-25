# Charts erstellen
---

?> Wenn du Video-Tutorials bevorzugst, hat NyxTheShield [ein Stream-Archiv](https://www.youtube.com/watch?v=ig27SlJveGs) dass jeden Schritt dieses Prozesses genau erklärt.

## Grundlagen
### Midi Editor/DAW
Charts werden erschaffen, wenn man eine midi Datei erstellt und sie mit dem Programm [Midi2TromboneChamp](#converting-midi-to-map-file) konvertiert.

Midi notes should be in the range 47 to 73 to match the game.<br>**NOTE:** Different editors use different values on the piano for this range.

Einige kostenlose, überprüfte Midi-Editoren beinhalten:
- [Reaper](https://www.reaper.fm/download.php)* (Range: B2-C#5)
- [LMMS](https://lmms.io/download#windows) (Range: B2-C#5)
- [FL Studio](https://www.image-line.com/fl-studio-download/)*† (Range: B3-C#6)
- [Cakewalk](https://www.bandlab.com/products/cakewalk)** (Range: B3-C#6)
- [Ableton](https://www.ableton.com/en/trial/)* (Range: B1-C#4)
- [Sekaiju](http://openmidiproject.osdn.jp/Sekaiju_en.html)
- [Trombone Charter](https://github.com/towai/TromboneCharter/releases/latest)

<sub>*Die vollständige Software ist nicht kostenlos, hat aber eine kostenlose Testversion.</sub><br> <sub>**Exportiert Noten normalerweise in der zweiten MIDI Spur, was es standardmäßig inkompatibel mit Midi2TromboneChamp macht.</sub><br> <sub>†Die Testversion von FL Studio erlaubt den Export von MIDI nicht aber Sie können dies umgehen, indem Sie die Projektdatei speichern und <a href="https://github.com/Kaydax/flp2midi/releases/latest">flp2midi</a> verwenden.</p>

<h4 spaces-before="0">
  Reaper Projekt
</h4>

<p spaces-before="0">
  Wenn du dir nicht sicher bist, welchen Editor du verwendet möchtest, wird Reaper empfohlen, da es eine benutzerdefinierte Trombone Champ Projektdatei gibt, die folgendes beinhaltet:
</p>

<ul>
  <li>
    Eine grundlegende Erklärung zur Verwendung der Steuerelemente von Reaper (in Englisch)
  </li>
  <li>
    Vorkonfigurierte Einstellungen
  </li>
  <li>
    MIDI Beispiele
  </li>
</ul>

<p spaces-before="0">
  Das Projekt kann <a href="https://trombone.wiki/docs/files/REAPER_Trombone_Champ_Charting_Template.zip">hier heruntergeladen werden</a>.
</p>

<h3 spaces-before="0">
  Normale Noten
</h3>

<p spaces-before="0">
  Normale Noten werden im Midi Editor erstellt und sehen im Spiel gleich aus. Achte darauf, immer einen kleinen Abstand zwischen den Noten zu lassen!
</p>

<h3 spaces-before="0">
  "Slide" Noten
</h3>

<p spaces-before="0">
  Slides are created by connecting notes with each other. The slide will start at the beginning of the first note and end at the end of the second note.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide1.png" alt="&quot;Slide&quot; Note Beispiel" />
</p>

<p spaces-before="0">
  To create slides with multiple parts or to adjust the slide timing and curve, split up the notes in the slide.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide2.png" alt="Mehrere &quot;Slide&quot; Noten Beispiel" />
</p>

<h2 spaces-before="0">
  Midi zum Chart konvertieren
</h2>

<ol start="1">
  <li>
    <p spaces-before="0">
      Go to <a href="https://tc-chart-converter.github.io/">Trombone Champ Chart Converter</a>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Füllen Sie die Felder aus:
    </p>
    <ul>
      <li>
        <code>Song Name</code> is the full name of the song, shown in the info when you select it in-game.
      </li>
      <li>
        <code>Short Name</code> wird beim Scrollen durch die Songliste angezeigt.
      </li>
      <li>
        <code>Artist</code> is the composer of the song.
      </li>
      <li>
        <code>Release Year</code> is the year the song was created.
      </li>
      <li>
        <code>Beats per Bar</code> bestimmt den Abstand zwischen den "beat lines".
      </li>
      <li>
        <code>Difficulty</code> ist die Anzahl der Schwierigkeitssterne, die in den Informationen des Songs erscheinen.
      </li>
      <li>
        <code>Note Spacing</code> kontrolliert zusammen mit BPM, wie schnell der Level scrollt.
      </li>
      <li>
        <code>trackRef</code> is the globally unique name used by mods to identify your chart.
      </li>
      <li>
        <code>Song Endpoint</code> ist die Nummer des Schlags, an dem der Song endet. Diese Nummer wird automatisch berechnet, allerdings kannst du sie ändern, um zu kontrollieren, wann der Level endet und der Endbildschirm erscheint.
      </li>
    </ul>
  </li>
  
  <li>
    <p spaces-before="0">
      Drücke OK. Create a folder with the same name as you entered in the <code>trackRef</code> field, and save the file as <code>song.tmb</code> inside that folder.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Dein Chart sollte eine .ogg Datei sein. Du kannst Programme wie Audacity benutzen, um Stille an den Anfang des Lieds zu setzen, sodass es gleichzeitig mit der Midi anfängt. Nenne die Datei <code>song.ogg</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Setze die.ogg Datei in den gleichen Ordner wie <code>song.tmb</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Folge der <a href="installing-songs">Anleitung zum Erstellen eigener Songs</a> um deinen Song zu testen.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      <a href="chart-backgrounds">Hintergrund hinzufügen!</a>
    </p>
  </li>
</ol>
