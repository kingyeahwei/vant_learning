<template>
  <div id="app">
    <van-cell title="选择日期区间" :value="date" @click="show = true"></van-cell>
    <van-calendar v-model="show" type="range" @confirm="onConfirm"></van-calendar>
  </div>
</template>

<script>
  import {Toast} from "vant"
  export default {
    name: 'App',
    data() {
      return {
        date: "",
        show: false
      }
    },
    methods: {
      formatDate(date) {
        return `${date.getMonth() + 1}/${date.getDate()}`
      },
      onConfirm(date) {
        const [start, end] = date;
        this.show = false;
        this.date = `${this.formatDate(start)} - ${this.formatDate(end)}`;
      }
    }
  }
</script>

<style>
</style>
