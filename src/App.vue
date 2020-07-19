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
        Toast("提示内容")
      }
    }
  }
</script>

<style>
</style>
