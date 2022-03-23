## Diatonic Chords

<div>
  <label><input type="radio" name="key" value="C" id="radioC">C</label>
  <label><input type="radio" name="key" value="D" id="radioD">D</label>
  <label><input type="radio" name="key" value="E" id="radioE">E</label>
  <label><input type="radio" name="key" value="F" id="radioF">F</label>
  <label><input type="radio" name="key" value="G" id="radioG">G</label>
  <label><input type="radio" name="key" value="A" id="radioA">A</label>
  <label><input type="radio" name="key" value="B" id="radioB">B</label>
</div>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
</style>

<table class="tg" id="targetTable">
<thead>
  <tr>
    <th class="tg-c3ow">Key</th>
    <th class="tg-c3ow">IM7</th>
    <th class="tg-c3ow">iim7</th>
    <th class="tg-c3ow">iiim7</th>
    <th class="tg-c3ow">IVM7</th>
    <th class="tg-c3ow">V7</th>
    <th class="tg-c3ow">vim7</th>
    <th class="tg-c3ow">viim7b5</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Root</td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Third</td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Fifth</td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Seventh</td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
    <td class="tg-c3ow"></td>
  </tr>
</tbody>
</table>

<script type="text/javascript">
  function valueChange(event){
    this.table.rows[1].cells[0].innerHTML = event.currentTarget.value;
    x = root.indexOf(event.currentTarget.value)
    y = tone.indexOf(event.currentTarget.value)
    for (let i = 0; i < 7; i++) {
      ix = (i+x)%7;
      this.table.rows[1].cells[i+1].innerHTML = this.root[ix] + this.list[i];
      for (let j = 0; j < 4; j++) {
        jy = (this.majmin[i][j]+y)%12;
        this.table.rows[j+2].cells[i+1].innerHTML = this.tone[jy];
      }
    }
  }
  
  const root = ['C', 'D', 'E', 'F', 'G', 'A', 'B']
  const list = ['M7', 'm7', 'm7', 'M7', '7', 'm7', 'm7b5']
  const tone = ['C', 'C#-D♭','D', 'D#-E♭','E','F', 'F#-G♭', 'G', 'G#-A♭', 'A', 'A#-B♭', 'B']
  const majmin = [[0, 4, 7, 11], [0, 3, 7, 10], [0, 3, 7, 10], [0, 4, 7, 11], [0, 4, 7, 10], [0, 3, 7, 10], [0, 3, 6, 10]]

  let table = document.getElementById('targetTable');

  let radioC = document.getElementById('radioC');
  radioC.checked = true;
  table.rows[1].cells[0].innerHTML = 'C'
  y = tone.indexOf('C');
  for (let i = 0; i < 7; i++) {
    table.rows[1].cells[i+1].innerHTML = root[i] + list[i];
    for (let j = 0; j < 4; j++) {
      jy = (majmin[i][j]+y)%12;
      table.rows[j+2].cells[i+1].innerHTML = tone[jy];
    }
  }
  radioC.addEventListener('change', {table: table, root: root, list: list, majmin: majmin, handleEvent: valueChange});

  let radioD = document.getElementById('radioD');
  radioD.addEventListener('change', {table: table, root: root, list: list, majmin: majmin, handleEvent: valueChange});

  let radioE = document.getElementById('radioE');
  radioE.addEventListener('change', {table: table, root: root, list: list, majmin: majmin, handleEvent: valueChange});

  let radioF = document.getElementById('radioF');
  radioF.addEventListener('change', {table: table, root: root, list: list, majmin: majmin, handleEvent: valueChange});

  let radioG = document.getElementById('radioG');
  radioG.addEventListener('change', {table: table, root: root, list: list, majmin: majmin, handleEvent: valueChange});

  let radioA = document.getElementById('radioA');
  radioA.addEventListener('change', {table: table, root: root, list: list, majmin: majmin, handleEvent: valueChange});

  let radioB = document.getElementById('radioB');
  radioB.addEventListener('change', {table: table, root: root, list: list, majmin: majmin, handleEvent: valueChange});
</script>
