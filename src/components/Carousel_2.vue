<script setup>

</script>

<template>
  <a-row>
    <a-col :span="8">
      <div style="height: 468px" class="card1_hover">
        <div class="card1"></div>
        <div style="padding: 32px 0;margin-right: 40px">
          <h4 style="margin-bottom: 8px">Get started fast</h4>
          <p style="color: #9797A2;font-size: 15px">
            Solo seller Megan Bre Camp started <b>Summer Solace</b> Tallow to sell her organic candles and skincare online and at local farmers markets.
          </p>
        </div>
      </div>
    </a-col>
    <a-col :span="8">
      <div style="height: 468px" class="card2_hover">
        <div class="card2"></div>
        <div style="padding: 32px 0;margin: 0 20px">
          <h4 style="margin-bottom: 8px">Grow as big as you want</h4>
          <p style="color: #9797A2;font-size: 15px">
            Athleisure brand <b>Gymshark</b> grew from working out of a garage to the global juggernaut it is today, with $500M+ sales annually.
          </p>
        </div>
      </div>
    </a-col>
    <a-col :span="8">
      <div style="height: 468px" class="card3_hover">
        <div class="card3"></div>
        <div style="padding: 32px 0;margin-left: 40px">
          <h4 style="margin-bottom: 8px">Raise the bar</h4>
          <p style="color: #9797A2;font-size: 15px">
            With the help of Shopify for enterprise, <b>Mattel</b> sells their iconic toys direct to customers around the world.
          </p>
        </div>
      </div>
    </a-col>
  </a-row>
</template>

<style scoped>
.card1 {
  height: 300px;
  margin-right: 40px;
  background: url("../assets/Section2/4ce35eba1e546a23ff875c3eba8b5705.webp") no-repeat center center /cover;
  border-radius: 10px;
  transition: background .5s;
}
.card2 {
  height: 300px;
  margin: 0 20px;
  background: url("../assets/Section2/2083b4178afc5db338c7d6081f8a5838.webp") no-repeat center center /cover;
  border-radius: 10px;
  transition: background .5s;
}
.card3 {
  height: 300px;
  margin-left: 40px;
  background: url("../assets/Section2/7c3d68ca99f2f743df8cb1187bbd2cb1.webp") no-repeat center center /cover;
  border-radius: 10px;
  transition: background .5s;
}

.card1_hover:hover .card1{
  background: url("../assets/Section2/ac93cea21424238e2231f2e0009da62e.webp") no-repeat center center /cover;
}
.card2_hover:hover .card2{
  background: url("../assets/Section2/07ae0290367bd34e86e56cdfeeae6846.webp") no-repeat center center /cover;
}
.card3_hover:hover .card3{
  background: url("../assets/Section2/22e30e7d8c99419f290192accf478f58.webp") no-repeat center center /cover;
}
</style>