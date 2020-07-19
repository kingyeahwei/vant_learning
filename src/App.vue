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
        show: false,
        toast: null
      }
    },
    methods: {
      handleClick() {
        this.$toast("提示文案")
      }
    }
  }
</script>

<style>
</style>
