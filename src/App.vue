<template>
  <div id="app">
    <van-button @click="handleClick">打开toast</van-button>
  </div>
</template>

<script>
  import {Toast} from "vant"
  export default {
    name: 'App',
    data() {
      return {
        show: false
      }
    },
    methods: {
      handleClick() {
        Toast.loading({
          message: "加载中...",
          // forbidClick: true,
          loadingType: "spinner"
        })
      }
    }
  }
</script>

<style>
</style>
