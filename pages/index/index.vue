<template>
  <view class="container">
    <text class="title">{{ message }}</text>
    <button @click="changeText">点击切换文字</button>
  </view>
</template>

<script setup>
import { ref } from 'vue'

const message = ref('Hello World')

const changeText = () => {
  message.value = 'Hello UniApp'
}
</script>

<style>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 100px;
}

.title {
  font-size: 24px;
  color: #333;
  margin-bottom: 20px;
}
</style>
