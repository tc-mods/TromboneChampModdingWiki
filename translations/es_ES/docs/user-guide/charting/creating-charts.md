# Creando Mapas
---

?> Si prefieres tutoriales en video, NyxTheShield tiene [un archivo de stream](https://www.youtube.com/watch?v=ig27SlJveGs) que explica cada paso del proceso de mapeado en detalle.

## Básicos
### Editor Midi/DAW
Los mapas se hacen creando un archivo midi y ejecutándolo en un [convertidor MIDI](#converting-midi-to-map-file).

Midi notes should be in the range 47 to 73 to match the game.<br>**NOTE:** Different editors use different values on the piano for this range.

Algunos editores midi gratis, verificados que funcionan incluyen:
- [Reaper](https://www.reaper.fm/download.php)* (Range: B2-C#5)
- [LMMS](https://lmms.io/download#windows) (Range: B2-C#5)
- [FL Studio](https://www.image-line.com/fl-studio-download/)*† (Range: B3-C#6)
- [Cakewalk](https://www.bandlab.com/products/cakewalk)** (Range: B3-C#6)
- [Ableton](https://www.ableton.com/en/trial/)* (Range: B1-C#4)
- [Sekaiju](http://openmidiproject.osdn.jp/Sekaiju_en.html)
- [Trombone Charter](https://github.com/towai/TromboneCharter/releases/latest)

<sub>*El software completo no es gratis, pero tiene una prueba gratuita wue funciona para mapear.</sub><br> <sub>**Exporta notas a pista MIDI 2 por defecto, que lo hace incompatible con Midi2TromboneChamp.</sub><br> <sub>†La versión de prueba de FL Studio no te deja exportar MIDI, pero puedes evitarlo al guardar el archivo del proyecto y usando <a href="https://github.com/Kaydax/flp2midi/releases/latest">flp2midi</a>.</p>

<h4 spaces-before="0">
  Proyecto Reaper
</h4>

<p spaces-before="0">
  Si no estás seguro de qué editor usar, Reaper es recomendable ya que hay un archivo de proyecto personalizado de Trombone Champ que viene con:
</p>

<ul>
  <li>
    Una explicación básica sobre cómo utilizar los controles de Reaper (en inglés)
  </li>
  <li>
    Ajustes preconfigurados
  </li>
  <li>
    MIDI de ejemplo
  </li>
</ul>

<p spaces-before="0">
  Este proyecto se puede <a href="https://trombone.wiki/docs/files/REAPER_Trombone_Champ_Charting_Template.zip">descargar aquí</a>.
</p>

<h3 spaces-before="0">
  Notas Normales
</h3>

<p spaces-before="0">
  Notas normales son creadas en el editor midi y se ven igualmente en el juego. ¡Asegúrate de dejar un tiempo de espacio entre notas!
</p>

<h3 spaces-before="0">
  Notas Deslizadas
</h3>

<p spaces-before="0">
  Slides are created by connecting notes with each other. The slide will start at the beginning of the first note and end at the end of the second note.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide1.png" alt="Ejemplo de nota deslizada" />
</p>

<p spaces-before="0">
  To create slides with multiple parts or to adjust the slide timing and curve, split up the notes in the slide.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide2.png" alt="Ejemplo de múltiples notas deslizadas" />
</p>

<h2 spaces-before="0">
  Convirtiendo Midi a Archivo de Mapa
</h2>

<ol start="1">
  <li>
    <p spaces-before="0">
      Go to <a href="https://tc-chart-converter.github.io/">Trombone Champ Chart Converter</a>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Rellena los campos:
    </p>
    <ul>
      <li>
        <code>Song Name</code> is the full name of the song, shown in the info when you select it in-game.
      </li>
      <li>
        <code>Short Name</code> se muestra mientras te desplazas por la lista de canciones.
      </li>
      <li>
        <code>Artist</code> is the composer of the song.
      </li>
      <li>
        <code>Release Year</code> is the year the song was created.
      </li>
      <li>
        <code>Beats per Bar</code> determina lo alejadas que están las "líneas de pulsos".
      </li>
      <li>
        <code>Difficulty</code> es el número de estrellas de dificultad que aparecen en la información de la canción.
      </li>
      <li>
        <code>Note Spacing</code> afecta cómo de rápido se desplaza el nivel, en combinación con BPM.
      </li>
      <li>
        <code>trackRef</code> is the globally unique name used by mods to identify your chart.
      </li>
      <li>
        <code>Song Endpoint</code> es el pulso en el que acaba la canción. Se calcula automáticamente, pero puedes ajustarlo para cambiar cuando aparece la pantalla del final de nivel.
      </li>
    </ul>
  </li>
  
  <li>
    <p spaces-before="0">
      Pulsa OK. Create a folder with the same name as you entered in the <code>trackRef</code> field, and save the file as <code>song.tmb</code> inside that folder.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Tu pista de música debería ser un archivo .ogg. Puedes usar software como Audacity para insertar silencio al principio de la pista que alinearla con el midi. Nombra al archivo <code>song.ogg</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Mueve el archivo ogg a la misma carpeta que <code>song.tmb</code>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      Sigue las <a href="installing-songs">Instrucciones de Instalación de Canciones Personalizadas</a> para probarlo.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      <a href="chart-backgrounds">¡Añade un fondo!</a>
    </p>
  </li>
</ol>
