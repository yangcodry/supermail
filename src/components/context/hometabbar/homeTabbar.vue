<template>
  <div class="tabbar">
    <tabbar>
      <tabbar-item path="/home">
        <img slot="tabbar-img" src="~assets/img/tabbar/home.svg" alt="">
        <img slot="tabbar-img-active" src="~assets/img/tabbar/home_active.svg" alt="">
        <span slot="word-name">主页</span>
      </tabbar-item>
      <tabbar-item path="/category">
        <img slot="tabbar-img" src="~assets/img/tabbar/category.svg" alt="">
        <img slot="tabbar-img-active" src="~assets/img/tabbar/category_active.svg" alt="">
        <span slot="word-name">分类</span>
      </tabbar-item>
      <tabbar-item path="/shopcart">
        <img slot="tabbar-img" src="~assets/img/tabbar/shopcart.svg" alt="">
        <img slot="tabbar-img-active" src="~assets/img/tabbar/shopcart_active.svg" alt="">
        <span slot="word-name">购物车</span>
      </tabbar-item>
      <tabbar-item path="/profile">
        <img slot="tabbar-img" src="~assets/img/tabbar/profile.svg" alt="">
        <img slot="tabbar-img-active" src="~assets/img/tabbar/profile_active.svg" alt="">
        <span slot="word-name">我的</span>
      </tabbar-item>
    </tabbar>
  </div>
</template>

<script>
  import Tabbar from "../../common/tabbar/Tabbar";
  import TabbarItem from "../../common/tabbar/TabbarItem";

  export default {
    name: "homeTabbar",
    components: {
      Tabbar,
      TabbarItem
    },
    data() {
      return {
      }
    }
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
  }

</style>
