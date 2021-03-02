<template>
  <div id="app">
    <home-tabbar></home-tabbar>
  </div>
</template>

<script>
import homeTabbar from "./components/context/hometabbar/homeTabbar";

export default {
  name: 'App',
  components: {
    homeTabbar
  }
}
</script>

<style>
#app {

}
</style>
