<script setup>
import MyMenu from "../components/MyMenu.vue";
import BodySection1 from "../components/BodySection1.vue";
import BodySection2 from "../components/BodySection2.vue";
</script>

<template>
  <a-layout id="layout">
    <a-layout-header class="header">
      <MyMenu />
    </a-layout-header>
    <a-layout-content class="body">
      <div>
        <BodySection1 class="content"/>
        <BodySection2 />
      </div>
    </a-layout-content>
  </a-layout>
</template>
<style scoped>




/* 脱离文本流，父元素相对于html（视窗） */
#layout .header {
  position: fixed;
  z-index :1;
  color: unset;
  background: unset;
  /* 将宽度设置视窗，且设置最大宽度，保证页面大小变化时自适应 */
  width: 100vw;
  max-width: 1420px;

  left: 50%; /* 相对于视口水平居中 */
  transform: translate(-50%, 0%); /* 相对于自身位置的调整，使其居中 */

}
#layout .content {
/**/
  position: relative;
  left: 50%; /* 相对于视口水平居中 */
  transform: translate(-50%, 0%); /* 相对于自身位置的调整，使其居中 */
  /* 将宽度设置视窗，且设置最大宽度，保证页面大小变化时自适应 */
  max-width: 1420px;
  width: 100vw;
}

</style>
