<script setup>

import Carousel_1 from "./Carousel_1.vue";
import Carousel_2 from "./Carousel_2.vue";
</script>

<template>
<div id="global_body2">
  <div class="first">
    The one commerce platform behind it all
    <div style="font-size: 40px;color: #7e7c7c;padding-bottom: 30px;">
      Sell online and in person. Sell locally and globally. Sell direct and wholesale. Sell on desktop and mobile.
    </div>
    <Carousel_1 />
  </div>
  <div class="second">
    <div style="padding-bottom: 30px;">
      <a-row>
        <a-col flex="800px">
          <div style="font-size: 40px;color: white">
            For everyone from entrepreneurs to enterprise
          </div>
        </a-col>
        <a-col flex="auto">
          <div class="te">
            Millions of merchants of every size have collectively<br>made over $1,000,000,000,000 in sales on Shopify.
          </div>
        </a-col>
      </a-row>
    </div>

    <Carousel_2 />
  </div>
</div>
</template>

<style scoped>
#global_body2{
  position: relative;
  bottom:100px;
  background: black;
  border-top-left-radius: 100px;
  border-top-right-radius: 100px;
  height: 2500px;
  padding-top: 50px;

}
.first{
  position: relative;
  left: 50%; /* 相对于视口水平居中 */
  transform: translate(-50%, 0%); /* 相对于自身位置的调整，使其居中 */
  max-width: 1420px;
  width: 100%;
  padding-left: 40px;
  font-size: 60px;
  color: white;
  padding-top: 30px;
  padding-right: 40px;
}

.second{
  position: relative;
  left: 50%; /* 相对于视口水平居中 */
  transform: translate(-50%, 0%); /* 相对于自身位置的调整，使其居中 */
  max-width: 1420px;
  width: 100%;
  padding-left: 40px;
  font-size: 60px;
  color: white;
  padding-top: 70px;
  padding-right: 40px;
}
.te{
  font-size: 15px;
  color: #9797A2;
  position: relative;
  top:50%;
}
@media (max-width: 1420px) {
  .first {
    max-width: unset;
  }
}
</style>