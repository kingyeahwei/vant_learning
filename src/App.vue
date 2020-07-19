<template>
  <div id="app">
    <van-cell title="选择多个日期" :value="text" @click="show = true"></van-cell>
    <van-calendar v-model="show" type="multiple" @confirm="onConfirm"></van-calendar>
  </div>
</template>

<script>
  import {Toast} from "vant"
  export default {
    name: 'App',
    data() {
      return {
        text: "",
        show: false
      }
    },
    methods: {
      onConfirm(date) {
        this.show = false;
        this.text = `选择了${date.length}个日期`;
      }
    }
  }
</script>

<style>
</style>
