<template>
  <h2 class="grid-title">5 X 5 基礎設定</h2>
  <div class="grid">
    <div class="red">
      <p>grid-row: 1 / 3;</p>
      <p>grid-column: 1 / 3;</p>
    </div>
    <div class="blue">
      <p>grid-row: 3 / 5;</p>
      <p>grid-column: 3/ 5;</p>
    </div>
    <div class="green">
      <p>grid-row: 1 / 6;</p>
      <p>grid-column: 5 / 6;</p>
    </div>
  </div>
  <p>grid-template-rows: 1fr 1fr 1fr 1fr 1fr;</p>
  <p>grid-template-columns: 1fr 1fr 1fr 1fr 1fr;</p>
</template>

<script>
export default {
  setup () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
.grid-title{
  background-color: #6e6e6e;
  font-size: 20px;
  line-height: 2;
  color: #fff;
}
.grid{
  width: 100%;
  height: 500px;
  display: grid;
  font-size: 20px;
  line-height: 2;
  grid-template-rows: repeat(5, 1fr);
  grid-template-columns: repeat(5, 1fr);
  color: #fff;
  .red{
    background-color: #f00;
    grid-row: 1 / 3;
    grid-column: 1 / 3;
  }
  .blue{
    background-color: blue;
    grid-row: 3 / 5;
    grid-column: 3/ 5;
  }
  .green{
    background-color: green;
    grid-row: 1 / 6;
    grid-column: 5 / 6;
  }
}
</style>