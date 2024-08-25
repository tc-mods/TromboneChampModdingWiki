# Karttojen Luonti
---

?> Jos haluat videotutoriaaleja, NyxTheShieldilla on [stream-arkisto](https://www.youtube.com/watch?v=ig27SlJveGs), joka selittää yksityiskohtaisesti kaikki kartoitusprosessin vaiheet.

## Perusteet
### Midi Editor/DAW
Kartat tehdään luomalla midi tiedosto ja viemällä ne [MIDI muuntimen](#converting-midi-to-map-file) läpi.

Midi notes should be in the range 47 to 73 to match the game.<br>**NOTE:** Different editors use different values on the piano for this range.

Jotkut ilmaiset, todennettu toimimaan midi editorit ovat:
- [Reaper](https://www.reaper.fm/download.php)* (Range: B2-C#5)
- [LMMS](https://lmms.io/download#windows) (Range: B2-C#5)
- [FL Studio](https://www.image-line.com/fl-studio-download/)*† (Range: B3-C#6)
- [Cakewalk](https://www.bandlab.com/products/cakewalk)** (Range: B3-C#6)
- [Ableton](https://www.ableton.com/en/trial/)* (Range: B1-C#4)
- [Sekaiju](http://openmidiproject.osdn.jp/Sekaiju_en.html)
- [Trombone Charter](https://github.com/towai/TromboneCharter/releases/latest)

<sub>*Täysi ohjelmisto ei ole ilmainen, mutta on ilmainen kokeiluversio, joka toimii kartoitukseen.</sub><br> <sub>**Vie nuotit MIDI radalle 2 oletuksena, mikä tekee siitä yhteensopimattoman Midi2TromboneChampin kanssa.</sub><br> <sub>†FL Studio kokeiluversio ei salli sinun viedä MIDIä mutta voit kiertää tämän tallentamalla projektin tiedoston ja käyttämällä <a href="https://github.com/Kaydax/flp2midi/releases/latest">flp2midi</a>.</p>

<h4 spaces-before="0">
  Reaper Projekti
</h4>

<p spaces-before="0">
  Jos et ole varma mitä editoria käyttäisi, Reaper on suositeltava, koska siinä on oma Trombone Champ projektitiedosto, joka sisältää:
</p>

<ul>
  <li>
    Perusselitys siitä, miten käyttää Reaperia (englanniksi)
  </li>
  <li>
    Esimääritellyt asetukset
  </li>
  <li>
    Esimerkki MIDI
  </li>
</ul>

<p spaces-before="0">
  Projekti voidaan <a href="https://trombone.wiki/docs/files/REAPER_Trombone_Champ_Charting_Template.zip">ladata täältä</a>.
</p>

<h3 spaces-before="0">
  Tavalliset Nuotit
</h3>

<p spaces-before="0">
  Normaalit nuotit luodaan midi editoriin ja näyttävät samalta pelin sisällä. Varmista, että jätät aukon nuottien väliin!
</p>

<h3 spaces-before="0">
  Liuku Nuotit
</h3>

<p spaces-before="0">
  Slides are created by connecting notes with each other. The slide will start at the beginning of the first note and end at the end of the second note.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide1.png" alt="Liuku Nuotti Esimerkki" />
</p>

<p spaces-before="0">
  To create slides with multiple parts or to adjust the slide timing and curve, split up the notes in the slide.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide2.png" alt="Useiden Liukunuottien Esimerkki" />
</p>

<h2 spaces-before="0">
  Muunnetaan Midi Karttatiedostoksi
</h2>

<ol start="1">
  <li>
    <p spaces-before="0">
      Go to <a href="https://tc-chart-converter.github.io/">Trombone Champ Chart Converter</a>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Täytä kentät:
    </p>
    <ul>
      <li>
        <code>Song Name</code> is the full name of the song, shown in the info when you select it in-game.
      </li>
      <li>
        <code>Short Name</code> näytetään kappalevalikossa.
      </li>
      <li>
        <code>Artist</code> is the composer of the song.
      </li>
      <li>
        <code>Release Year</code> is the year the song was created.
      </li>
      <li>
        <code>Beats per Bar</code> määrittää, kuinka kaukana "iskulinjat" ovat.
      </li>
      <li>
        <code>Difficulty</code> on vaikeustaso eli tähtien määrä, jotka näkyvät kappaleen tiedoissa.
      </li>
      <li>
        <code>Note Spacing</code> vaikuttaa siihen, kuinka nopeasti taso rullaa yhdessä BPM kanssa.
      </li>
      <li>
        <code>trackRef</code> is the globally unique name used by mods to identify your chart.
      </li>
      <li>
        <code>Song Endpoint</code> on isku, jolla kappale päättyy. Se lasketaan automaattisesti, mutta voit säätää sitä muuttaaksesi, kun tason loppunäyttö näkyy.
      </li>
    </ul>
  </li>
  
  <li>
    <p spaces-before="0">
      Paina OK. Create a folder with the same name as you entered in the <code>trackRef</code> field, and save the file as <code>song.tmb</code> inside that folder.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Musiikkikappaleesi pitäisi olla .ogg-tiedosto. Voit käyttää Audacityn kaltaista ohjelmistoa asettaksesi hiljaisuuden kappaleen alkuun, jotta voit saada sen syncaamaan midin kanssa. Nimeä tiedosto <code>song.ogg</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Siirrä ogg-tiedosto samaan kansioon kuin <code>song.tmb</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Testaa sitä noudattamalla <a href="installing-songs">Custom kappaleen asennusohjeita</a>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      <a href="chart-backgrounds">Lisää tausta!</a>
    </p>
  </li>
</ol>
