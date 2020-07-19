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
        Toast.allowMultiple();
        const toast1 = Toast("第一个 Toast");
        const toast2 = Toast.success("第二个 Toast");
        setTimeout(() => {
          toast1.clear()
          toast2.clear()
        }, 3000)
      }
    }
  }
</script>

<style>
</style>
