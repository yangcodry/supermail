<template>
  <div class="tabbar-item tabbar-self" @click="activeClick">
    <slot v-if="isActive" name="tabbar-img"></slot>
    <slot v-else name="tabbar-img-active"></slot>
    <div class="word-size" :style="wordColor">
      <slot name="word-name"></slot>
    </div>
  </div>
</template>

<script>
  export default {
    name: "TabbarItem",
    props: {
      path: {
        type: String
      }
    },
    data() {
      return {
        //isActive: true,
      }
    },
    computed: {
      wordColor() {
        return this.isActive ? {} : {color: 'red'}
      },
      isActive() {
        return !(this.$route.path == this.path)
      }
    },
    methods: {
      activeClick() {
        if(this.$route.path != this.path) {
          this.$router.push(this.path)
        }
      }
    }
  }
</script>

<style scoped>
  .tabbar-item {
    background: white;
    flex: 1;
  }
  .tabbar-self {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .tabbar-item img {
    width: 24px;
    height: 24px;
  }
  .word-size {
    font-size: 14px;
    margin-top: 3px;
  }
</style>
