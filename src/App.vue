<template>
  <h1 class="title">{{title}}</h1>
  <router-view></router-view>
</template>

<script>
export default {
  setup () {
    return {
      title: 'Grid css 練習計畫'
    }
  }
}
</script>


<style lang="scss">
#app {
  font-family: 'openhuninn', 'Noto Sans TC', sans-serif;
  text-align: center;
}
.title{
  font-size: 30px;
  line-height: 1.9;
  background-color: #333;
  color: #fff;
}
</style>
