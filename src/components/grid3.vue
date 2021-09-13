<template>
  <h2 class="grid-title">5 X 5 + 區塊命名</h2>
  <div class="grid">
    <div class="red">
      <p>grid-area: header;</p>
    </div>
    <div class="blue">
      <p>grid-area: nav;</p>
    </div>
    <div class="green">
      <p>grid-area: main;</p>
    </div>
    <div class="black">
      <p>grid-area: footer;</p>
    </div>
  </div>
  <p>grid-template-rows: 1fr 1fr 1fr 1fr 1fr;</p>
  <p>grid-template-columns: 1fr 1fr 1fr 1fr 1fr;</p>
  <p>grid-template-areas: "header header header header header"
    "nav main main main main"
    "nav main main main main"
    "nav main main main main"
    ". footer footer footer .";</p>
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
  grid-template-areas: "header header header header header"
    "nav main main main main"
    "nav main main main main"
    "nav main main main main"
    ". footer footer footer .";
  color: #fff;
  .red{
    background-color: #f00;
    grid-area: header;
  }
  .blue{
    background-color: blue;
    grid-area: nav;
  }
  .green{
    background-color: green;
    grid-area: main;
  }
  .black{
    background-color: black;
    grid-area: footer;
  }
}
</style>