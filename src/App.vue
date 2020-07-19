<template>
  <div id="app">
    <van-button @click="show = true">点击</van-button>
    <van-calendar v-model="show" type="range" confirm-text="完成" confirm-disabled-text="快选择呀"></van-calendar>
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
      onConfirm(date) {
        console.log(date)
        this.show = false;
      }
    }
  }
</script>

<style>
</style>
