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
        // Toast.success("成功文案");
        Toast.fail("失败文案");
      }
    }
  }
</script>

<style>
</style>
