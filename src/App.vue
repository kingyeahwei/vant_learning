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
        // Toast({
        //   message: "自定义图标",
        //   icon: "like-o"
        // })
        Toast({
          message: "展示图片",
          icon: "https://img.yzcdn.cn/vant/logo.png"
        })
      }
    }
  }
</script>

<style>
</style>
