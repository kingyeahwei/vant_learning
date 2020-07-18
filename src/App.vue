<template>
  <div id="app">
    <div style="height: 10px"></div>
    <van-cell value="内容" is-link>
      <template #title>
        <span class="custom-title">单元格</span>
        <van-tag type="danger">标签</van-tag>
      </template>
    </van-cell>
    <van-cell title="单元格" icon="shop-o">
      <template #right-icon>
        <van-icon name="search" style="font-size: 16px; line-height: inherit;"></van-icon>
      </template>
    </van-cell>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
</style>
