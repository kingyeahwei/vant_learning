<template>
  <div id="app">
    <div style="height: 10px"></div>
    <van-cell-group>
      <van-cell title="URL 跳转" is-link url="/vant/mobile.html"></van-cell>
      <van-cell title="路由跳转" is-link to="index"></van-cell>
    </van-cell-group>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
</style>
