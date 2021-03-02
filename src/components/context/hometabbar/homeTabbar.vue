<template>
  <div class="tabbar">
    <div class="tabbar-item"></div>
    <div class="tabbar-item"></div>
    <div class="tabbar-item"></div>
    <div class="tabbar-item"></div>
  </div>
</template>

<script>
  export default {
    name: "homeTabbar"
  }
</script>

<style scoped>
  .tabbar {
    width: 49px;
    display: flex;
    margin-left: 0;
    margin-right: 0;
    margin-bottom: 0;
    position:fixed;
  }
  .tabbar-item {
    background: yellow;
    flex: 1;
  }
</style>
