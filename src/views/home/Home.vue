<template>
  <div>
    <nav-bar class="nav-bar">
      <span slot="center-navbar">主页</span>
    </nav-bar>
    <div>主页</div>
  </div>
</template>

<script>
  import NavBar from "@/components/common/navbar/NavBar";

  export default {
    name: "Home",
    components: {
      NavBar
    }
  }
</script>

<style scoped>
  .nav-bar {
    background-color: pink;
    text-align: center;
  }
</style>
