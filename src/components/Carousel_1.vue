<template>
  <a-carousel autoplay :dots="false">
    <div>
      <a-row>
        <a-col :span="9">
          <div class="OIP-C"></div>
        </a-col>
        <a-col :span="6">
          <div class="OIP-C1"></div>
        </a-col>
        <a-col :span="9">
          <div class="OIP-C2"></div>
        </a-col>
      </a-row>
    </div>
    <div>
      <a-row>
        <a-col :span="9">
          <div class="OIP-C3"></div>
        </a-col>
        <a-col :span="6">
          <div class="OIP-C4"></div>
        </a-col>
        <a-col :span="9">
          <div class="OIP-C5"></div>
        </a-col>
      </a-row>
    </div>
    <div>
      <a-row>
        <a-col :span="9">
          <div class="OIP-C6"></div>
        </a-col>
        <a-col :span="6">
          <div class="OIP-C7"></div>
        </a-col>
        <a-col :span="9">
          <div class="OIP-C8"></div>
        </a-col>
      </a-row>
    </div>


  </a-carousel>
</template>

<style scoped>
/* For demo */
:deep(.slick-slide) {
  text-align: center;
  height: 400px;
  line-height: 160px;
  background: #364d79;
  overflow: hidden;
  border-radius: 10px;

}
:deep(.slick-slide h3) {
  color: #fff;
}

div{
  height: 400px;
  border-radius: 10px;
}


.OIP-C{
  background: url("../assets/Animation/sakura/OIP-C.jpg") no-repeat center center /cover;
  margin-right: 10px;
}
.OIP-C2{
  background: url("../assets/Animation/sakura/OIP-C (2).jpg") no-repeat center center /cover;
  margin-left: 10px;
}
.OIP-C1{
  background: url("../assets/Animation/sakura/OIP-C (1).jpg") no-repeat center center /cover;
}

.OIP-C3{
  background: url("../assets/Animation/star/OIP-C (4).jpg") no-repeat center center /cover;
  margin-right: 10px;
}
.OIP-C4{
  background: url("../assets/Animation/star/OIP-C.jpg") no-repeat center center /cover;
}
.OIP-C5{
  background: url("../assets/Animation/star/OIP-C4.jpeg") no-repeat center center /cover;
  margin-left: 10px;
}

.OIP-C6{
  background: url("../assets/Animation/text/OIP-C (2).jpg") no-repeat center center /cover;
  margin-right: 10px;
}
.OIP-C7{
  background: url("../assets/Animation/text/adwa.jpg") no-repeat center center /cover;
}
.OIP-C8{
  background: url("../assets/Animation/text/OIP-C (1).jpg") no-repeat center center /cover;
  margin-left: 10px;

}

</style>
<script setup lang="ts">
</script>