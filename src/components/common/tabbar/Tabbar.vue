<template>
  <div class="tabbar">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    name: "Tabbar"
  }
</script>

<style scoped>
  .tabbar {
    height: 49px;
    display: flex;
    left: 0;
    right: 0;
    bottom: 0;
    position:fixed;
    box-shadow: 0px -1px 1px rgba(100,100,100,.1)
  }
</style>
