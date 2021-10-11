<template>
  <div id="app">
    <router-view></router-view>
    <home-tabbar></home-tabbar>
  </div>
</template>

<script>
import homeTabbar from "components/context/hometabbar/homeTabbar";

export default {
  name: 'App',
  components: {
    homeTabbar
  }
}
</script>

<style>
  @import './assets/css/base.css';
#app {

}
</style>
