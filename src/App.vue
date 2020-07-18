<template>
  <div id="app">
    <van-image src="https://img.yzcdn.cn/vant/cat.jpeg">
      <template v-slot:loading>
        <van-loading type="spinner" size="20"></van-loading>
      </template>
    </van-image>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
</style>
