<template>
  <div id="app">
    <van-button @click="showPopup">弹出</van-button>
    <!--<van-popup v-model="show" closeable position="bottom" :style="{height: '60%'}"></van-popup>-->
    <!--<van-popup-->
    <!--  v-model="show"-->
    <!--  closeable-->
    <!--  close-icon="close"-->
    <!--  position="bottom"-->
    <!--  :style="{ height: '30%' }"-->
    <!--/>-->

    <van-popup
      v-model="show"
      closeable
      close-icon-position="top-left"
      position="bottom"
      round
      :style="{height: '30%'}"
    ></van-popup>
  </div>
</template>

<script>
  export default {
    name: 'App',
    data() {
      return {
        show: false
      }
    },
    methods: {
      showPopup() {
        this.show = true;
      }
    }
  }
</script>

<style>
</style>
