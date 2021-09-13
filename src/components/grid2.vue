<template>
  <h2 class="grid-title">5 X 5 + 隔線命名</h2>
  <div class="grid">
    <div class="red">
      <p>grid-row: Y1 / Y4;</p>
      <p>grid-column: X1 / X2;</p>
    </div>
    <div class="blue">
      <p>grid-row: Y2 / Y5;</p>
      <p>grid-column: X3/ X4;</p>
    </div>
    <div class="green">
      <p>grid-row: Y1 / Y4;</p>
      <p>grid-column: X4 / X6;</p>
    </div>
  </div>
  <p>grid-template-rows: [Y1] 1fr [Y2] 1fr [Y3] 1fr [Y4] 1fr [Y5] 1fr [Y6];</p>
  <p>grid-template-columns: [X1] 1fr [X2] 1fr [X3] 1fr [X4] 1fr [X5] 1fr [X6];</p>
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
  grid-template-rows: [Y1] 1fr [Y2] 1fr [Y3] 1fr [Y4] 1fr [Y5] 1fr [Y6];
  grid-template-columns: [X1] 1fr [X2] 1fr [X3] 1fr [X4] 1fr [X5] 1fr [X6];
  color: #fff;
  .red{
    background-color: #f00;
    grid-row: Y1 / Y4;
    grid-column: X1 / X2;
  }
  .blue{
    background-color: blue;
    grid-row: Y2 / Y5;
    grid-column: X3/ X4;
  }
  .green{
    background-color: green;
    grid-row: Y1 / Y4;
    grid-column: X4 / X6;
  }
}
</style>