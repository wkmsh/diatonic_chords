## Diatonic Chords

|   Key   | IM7 | iim7 | iiim7 | IVM7 | V7 | vim7 | viim7b5 |
|:-------:|:---:|:----:|:-----:|:----:|:--:|:----:|:-------:|
|         |     |      |       |      |    |      |         |
|   Root  |     |      |       |      |    |      |         |
|  Third  |     |      |       |      |    |      |         |
|  Fifth  |     |      |       |      |    |      |         |
| Seventh |     |      |       |      |    |      |         |

<div>
<label><input type="radio" name="key" value="c" id="radioC">C</label>
<label><input type="radio" name="key" value="d" id="radioD">D</label>
<label><input type="radio" name="key" value="e" id="radioE">E</label>
<label><input type="radio" name="key" value="f" id="radioF">F</label>
<label><input type="radio" name="key" value="g" id="radioG">G</label>
<label><input type="radio" name="key" value="a" id="radioA">A</label>
<label><input type="radio" name="key" value="b" id="radioB">B</label>
</div>

<script type="text/javascript">
  function valueChange(event, table){
    console.log('選択されているのは ' + event.currentTarget.value + ' です');
    table.rows[1].cells[0].innerHTML = event.currentTarget.value
  }

  let table = document.getElementById('targetTable');
  document.getElementById('targetTable');

  let radioC = document.getElementById('radioC');
  radioC.checked = true;
  radioC.addEventListener('change', valueChange);

  let radioD = document.getElementById('radioD');
  radioD.addEventListener('change', valueChange);

  let radioE = document.getElementById('radioE');
  radioE.addEventListener('change', valueChange);

  let radioF = document.getElementById('radioF');
  radioF.addEventListener('change', valueChange);

  let radioG = document.getElementById('radioG');
  radioG.addEventListener('change', valueChange);

  let radioA = document.getElementById('radioA');
  radioA.addEventListener('change', valueChange);

  let radioB = document.getElementById('radioB');
  radioB.addEventListener('change', valueChange);
</script>

<div>
  <label><input type="radio" name="key" value="c">C</label>
  <label><input type="radio" name="key" value="d">D</label>
  <label><input type="radio" name="key" value="e">E</label>
  <label><input type="radio" name="key" value="f">F</label>
  <label><input type="radio" name="key" value="g">G</label>
  <label><input type="radio" name="key" value="a">A</label>
  <label><input type="radio" name="key" value="b">B</label>
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
