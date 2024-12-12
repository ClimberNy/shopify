<script setup>

import { ref, onMounted, onUnmounted } from 'vue';



const status = ref('big thing'); // 初始值
const values = ['one to watch', 'category creator', 'unicorn startup', 'household name', 'global empire', 'solo flier', 'store they line','big thing']; // 三种值的数组
let currentIndex = 0; // 当前值的索引
// 更新状态的函数
const updateStatus = () => {
  status.value = values[currentIndex];
  currentIndex = (currentIndex + 1) % values.length; // 循环到下一个值
};
// 组件挂载时设置定时器
onMounted(() => {
  const intervalId = setInterval(updateStatus, 3500); // 每秒更新一次状态
  // 组件卸载时清除定时器
  onUnmounted(() => {
    clearInterval(intervalId);
  });
});
</script>

<template>

  <div id="global_body1">
    <video autoplay loop muted playsinline>
      <source src="../assets/background.mp4" type="video/mp4" />
    </video>

    <div class="all_text">
      <span>
        Be the next<br>{{ status }}
      </span>
      <div class="test_2">
        Dream big, build fast, and<br>grow far on Shopify.
      </div>
      <div class="part_3">
        <a-row>
          <a-col flex="100px">
            <a-button class="start_2" type="primary">Start free trial</a-button>
          </a-col>
          <a-col flex="auto">
            <div style="padding-left: 30px">
              Get 3 days free<br>then 1 month for $1
            </div>
          </a-col>
          <a-col flex="100px">
            <a-button class="reason" type="primary">Why we build shopify</a-button>
          </a-col>
        </a-row>

      </div>


    </div>
  </div>
<!--  网络原因-->
<!--  <video aria-label="Shopify 商家开展销售、管理业务和庆祝成功的视频素材" autoplay="" class="absolute size-full object-cover" loop="" playsinline="" src="blob:https://www.shopify.com/0b1e875e-c87a-4127-bcbb-65933797c35e"></video>-->
</template>

<style scoped>
@media (max-width: 1420px) {
  video {
    min-width: unset;
  }
}
#global_body1 {
  height:700px;
  width: 100vw;
}
video {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: -100;
  width: 100vw;
  min-width: 1420px;
  max-width: 6051px;
  overflow: hidden;
}
#global_body1 .all_text{
  position: relative;
  top:20%;
  color:white;
  font-size: 70px;
  padding-left: 40px;
  padding-right: 40px;
}
#global_body1 .test_2{
  font-size: 20px;
  padding-top: 20px;
}

#global_body1 .part_3{
  padding-top:30px;
}

.start_2{
  background: white;
  padding: 4px 30px;
  border: 0;
  color: black;
  border-radius: 20px;
  width: 150px;
  height: 40px;
}
.start_2:hover{
  background: #ececec;
}

.reason{
  margin-right: 20px;
  border-radius: 20px;
  background: transparent;
  border: 0;
  height: 40px;
  font-size: 20px;
}
.reason:hover{
  background: #7e7d7d;
  opacity: 0.5;
}
</style>