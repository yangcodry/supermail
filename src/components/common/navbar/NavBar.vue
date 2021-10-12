<template>
  <div class="navbar">
    <div class="left"><slot name="left-navbar"></slot></div>
    <div class="center"><slot name="center-navbar"></slot></div>
    <div class="right"><slot name="right-navbar"></slot></div>
  </div>
</template>

<script>
  export default {
    name: "NavBar"
  }
</script>

<style scoped>
  .navbar {
    display: flex;
    height: 44px;
    line-height: 44px;
    box-shadow: 0px 1px 1px rgba(100,100,100,.1)
  }
  .left {
    width: 40px;
  }
  .center {
    flex: 1;
  }
  .right {
    width: 40px;
  }
</style>
