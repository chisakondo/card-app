<template>
  <!-- 名刺デザイン16 -->
  <div class="absolute c-design w-full h-full">
    <div class="c-type8 absolute" style="width: 85%; height: 85%;"></div>
  </div>
</template>

<script>
export default {}
</script>
<style scoped>
/* レスポンシブを考えると%指定が望ましい */
.c-design {
  top: 0;
}
.c-type8 {
  right: 3%;
  bottom: 3%;
  background-image: url("~assets/images/templates/template4/bgObject4.png");
  background-size: contain;
  background-repeat: no-repeat;
  background-position-x: 100%;
}
</style>
