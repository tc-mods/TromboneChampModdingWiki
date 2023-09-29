# Map Maken
---

?> Als je liever en videotutorial wil hebben, heeft NyxTheShield een [en streamarchief](https://www.youtube.com/watch?v=ig27SlJveGs) waarin elke stap van het maken van een map in detail wordt uitgelegd. Opmerking: de video is in het Engels.

## Basiskennis
### MIDI Editor/DAW
Maps zijn gemaakt door een MIDI bestand te maken en deze door [Midi2TromboneChamp](#converting-midi-to-map-file) te voeren.

Midi notes should be in the range 47 to 73 to match the game.<br>**NOTE:** Different editors use different values on the piano for this range.

Enkele gratis en geverifieerd werkende MIDI-editors zijn:
- [Reaper](https://www.reaper.fm/download.php)* (Range: B2-C#5)
- [LMMS](https://lmms.io/download#windows) (Range: B2-C#5)
- [FL Studio](https://www.image-line.com/fl-studio-download/)*† (Range: B3-C#6)
- [Cakewalk](https://www.bandlab.com/products/cakewalk)** (Range: B3-C#6)
- [Ableton](https://www.ableton.com/en/trial/)* (Range: B1-C#4)
- [Sekaiju](http://openmidiproject.osdn.jp/Sekaiju_en.html)
- [Trombone Charter](https://github.com/towai/TromboneCharter/releases/latest)

<sub>* Volledige software is niet gratis, maar er is wel een gratis proefversie die werkt voor het maken van maps.</sub><br> <sub>**Exporteert notities standaard in MIDI track 2, wat het incompatibel maakt met Midi2TromboneChamp.</sub><br> <sub>† De proefversie van FL Studio staat niet toe MIDI te exporteren. Je kan dit omzeilen door het projectbestand op te slaan en <a href="https://github.com/Kaydax/flp2midi/releases/latest">flp2midi</a> te gebruiken.</p>

<h4 spaces-before="0">
  Reaper Project
</h4>

<p spaces-before="0">
  Als je niet zeker weet welke editor je wil gebruiken wordt Reaper aanbevolen omdat er een vooraf gemaakt Trombone Champ-projectbestand is. Dit bestand omvat:
</p>

<ul>
  <li>
    Een basisuitleg over het gebruik van de besturingselementen van Reaper (in het Engels)
  </li>
  <li>
    Vooraf geconfigureerde instellingen
  </li>
  <li>
    Voorbeeld MIDI
  </li>
</ul>

<p spaces-before="0">
  Het project kan hier <a href="https://trombone.wiki/docs/files/REAPER_Trombone_Champ_Charting_Template.zip">gedownload worden</a>.
</p>

<h3 spaces-before="0">
  Normale Noten
</h3>

<p spaces-before="0">
  Normale noten worden gemaakt in de MIDI-editor en zien er in-game hetzelfde uit. Zorg ervoor dat je ruimte overlaat tussen de noten!
</p>

<h3 spaces-before="0">
  Schuifnoten
</h3>

<p spaces-before="0">
  Schuifnoten worden gemaakt door overlappende noten in de tijd. Voor een paar overlappende noten gaat de schuif van het begin van de eerste noot naar het begin van de tweede. Het overlappende deel van de eerste noot wordt achterwege gelaten. Bekijk deze afbeelding voor een voorbeeld:
</p>

<p spaces-before="0">
  <img src="../docs/files/slide1.png" alt="Schuifnoot Voorbeeld" />
</p>

<p spaces-before="0">
  Als een noot eindigt, maar de volgende noot op hetzelfde moment begint, worden ze aaneengesloten. Hiermee kun je de curve aanpassen waar een schuifnoot start. Hier volgt een voorbeeld van meerdere schuifnoten die met elkaar zijn verbonden:
</p>

<p spaces-before="0">
  (Let op: het eerste rechte gedeelte is een aparte noot uit het gebogen gedeelte. De eindtijd is gelijk aan de begintijd van de volgende noot.)
</p>

<p spaces-before="0">
  <img src="../docs/files/slide2.png" alt="Voorbeeld van meervoudige schuifnoten" />
</p>

<h2 spaces-before="0">
  MIDI omzetten naar een map bestand
</h2>

<ol start="1">
  <li>
    <p spaces-before="0">
      Go to <a href="https://tc-chart-converter.github.io/">Trombone Champ Chart Converter</a>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Vul de velden in:
    </p>
    <ul>
      <li>
        <code>Song Name</code> is the full name of the song, shown in the info when you select it in-game.
      </li>
      <li>
        <code>Short Name</code> wordt weergeven tijdens het scrollen door de songlijst. Deze text wordt kleiner te langer de naam is, dus ik weet niet of er een maximale lengte is.
      </li>
      <li>
        <code>Release Year</code> is the year the song was created.
      </li>
      <li>
        <code>Artist</code> is the composer of the song.
      </li>
      <li>
        <code>Beats per Bar</code> bepaalt hoe ver de "beat lines" uit elkaar staan.
      </li>
      <li>
        <code>Difficulty</code> is het aantal moeilijkheidssterren dat op de info van de map verschijnt.
      </li>
      <li>
        <code>Note Spacing</code> beïnvloedt in combinatie met de BPM hoe snel het level scrollt.
      </li>
      <li>
        <code>Folder Name</code> is de naam van de map waarin je de map en audiobestand wil plaatsen. Bijv. Als je de mapnaam op mijn map zet, zal het pad van de map BepInEx/CustomSongs/mijn map/song.tmb zijn.
      </li>
      <li>
        <code>Song Endpoint</code> is de beat waarop het nummer eindigt. Het wordt automatisch berekend, maar je kan het aanpassen om het moment dat het eindscherm in beeld komt te veranderen.
      </li>
    </ul>
  </li>
  
  <li>
    <p spaces-before="0">
      Klik op OK. Create a folder with the same name as you entered in the <code>Folder Name</code> field, and save the file as <code>song.tmb</code> inside that folder.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      De gebruikte muziek moet een .ogg bestand zijn. Op het moment van schrijven moet de duur van de track langer zijn dan het Song Endpoint, of het nummer zal vastlopen en nooit eindigen. Je kunt software als Audacity gebruiken om stilte in te voegen aan het begin van het liedje om het met synchroon te laten lopen met de MIDI. Noem het bestand <code>song.ogg</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Verplaats het ogg-bestand naar dezelfde map als <code>song.tmb</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Volg de <a href="installing-songs">Liedjes Installeren handleiding</a> om het te testen.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      <a href="chart-backgrounds">Voeg een achtergrond toe!</a>
    </p>
  </li>
</ol>
