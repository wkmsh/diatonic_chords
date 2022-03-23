## Diatonic Chords

<div>
  <label><input type="radio" name="key" value="c">C</label>
  <label><input type="radio" name="key" value="d">D</label>
  <label><input type="radio" name="key" value="e">E</label>
</div>

|   Key   | IM7 | iim7 | iiim7 | IVM7 | V7 | vim7 | viim7b5 |
|:-------:|:---:|:----:|:-----:|:----:|:--:|:----:|:-------:|
|         |     |      |       |      |    |      |         |
|   Root  |     |      |       |      |    |      |         |
|  Third  |     |      |       |      |    |      |         |
|  Fifth  |     |      |       |      |    |      |         |
| Seventh |     |      |       |      |    |      |         |

<table id="targetTable">
  <thead>
    <tr>
      <td>名前</td>
      <td>年齢</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>鈴木</td>
      <td>14</td>
    </tr>
    <tr>
      <td>山田</td>
      <td>18</td>
    </tr>
  <tbody>
</table>

<script type="text/javascript">
  let table = document.getElementById('targetTable');

  for (let row of table.rows) {
      for(let cell of row.cells){
         console.log(cell.innerText);
      }
  }
  
  table.rows[1].cells[1].innerHTML = 'moji'
</script>
