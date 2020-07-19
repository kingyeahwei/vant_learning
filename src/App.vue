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
        const toast = Toast.loading({
          duration: 3000,
          forbidClick: true,
          message: "倒计时3秒"
        })
        let second = 3;
        const timer = setInterval(() => {
          second--;
          if (second) {
            toast.message = `倒计时${second} 秒`
          } else {
            clearInterval(timer);
            Toast.clear()
          }
        }, 1000)
      }
    }
  }
</script>

<style>
</style>
