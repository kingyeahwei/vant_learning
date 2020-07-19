<template>
  <div id="app">
    <van-cell is-link @click="showPopup">展示弹出层</van-cell>
    <van-popup v-model="show" position="right">内容</van-popup>
  </div>
</template>

<script>
  export default {
    name: 'App',
    data() {
      return {
        show: false
      }
    },
    methods: {
      showPopup() {
        this.show = true;
      }
    }
  }
</script>

<style>
</style>
