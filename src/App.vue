<script setup>
import LayOut from "./Layouts/LayOut.vue";

import { ref, onMounted, onUnmounted } from 'vue';

const backgroundColor = ref('transparent'); // 默认背景色为透明

// 监听页面滚动事件
const handleScroll = () => {
  if (window.scrollY > 0) {
    backgroundColor.value = '#000'; // 页面不在顶部时背景色变为黑色
  } else {
    backgroundColor.value = 'transparent'; // 页面在顶部时背景色为透明
  }
};

// 在组件挂载后添加事件监听器
onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

// 在组件卸载前移除事件监听器
onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>



<template>
  <div class="scroll" :style="{ backgroundColor: backgroundColor }"></div>
  <LayOut />
</template>

<style scoped>
.scroll{
  position: fixed;
  width: 100%;
  height: 64px;
  z-index: 1;
}
</style>
