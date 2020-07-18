<template>
  <div id="app">
    <van-image src="https://img.yzcdn.cn/vant/cat.jpeg">
      <template v-slot:error>加载失败</template>
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
