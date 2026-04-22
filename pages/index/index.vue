<template>
  <view class="container">
    <web-view :src="webUrl"></web-view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      webUrl: './index.html'
    }
  }
}
</script>

<style>
.container {
  width: 100%;
  height: 100vh;
  overflow: hidden;
}
</style>
