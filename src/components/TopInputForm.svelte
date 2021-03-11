<script lang="ts">

  let priceType = 'etc'
  const onSearch = () => {
    console.log('hpge')
  }
</script>

<style lang="scss">
input {
  border: 1px solid #bda213;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  border-radius: 4px;
  padding: 8px 12px;
}
button {
  border: 1px solid green;
  background-color: green;
  color: white;
  font-weight: bold;
  border-radius: 4px;
  &:hover {
    cursor: pointer;
  }
}
</style>

<div>ドライブルートを入力してください</div>

<table>
  <tbody>
    <tr>
      <td><input type="text" placeholder="出発地点" /></td>
      <td>　〜　</td>
      <td><input type="text" placeholder="到着地点" /></td>
    </tr>
  </tbody>
</table>

<div>中継地点①を入力してください</div>

<input type="text" placeholder="中間地点" />

<div>ドライブ人数を入力してください</div>

<input type="number" placeholder="1" />

<div>高速料金支払いタイプを選んで下さい</div>

<div>
  <input type="radio" name="priceType" value="etc" group="{priceType}" checked="{true}">ETC
  <input type="radio" name="priceType" value="cash">現金
</div>

<button on:click={onSearch}>検索する</button>