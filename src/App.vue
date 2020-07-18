<template>
  <div id="app">
    <div style="height: 10px"></div>
    <van-cell-group>
      <van-cell title="单元格" is-link></van-cell>
      <van-cell title="单元格" is-link value="内容"></van-cell>
      <van-cell title="单元格" is-link arrow-direction="down" value="内容"></van-cell>
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
