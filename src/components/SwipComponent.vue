<template>
    <div class="swiper">
        <mt-swipe :auto="5000" :show-indicators="false" >
  <mt-swipe-item>
      <a href="javascript:void(0)">
          <img src="../assets/images/lb1.jpg" alt="">
      </a>
  </mt-swipe-item>
  <mt-swipe-item><a href="javascript:void(0)">
          <img src="../assets/images/lb2.jpg" alt="">
      </a></mt-swipe-item>
  <mt-swipe-item><a href="javascript:void(0)">
          <img src="../assets/images/lb3.jpg" alt="">
      </a></mt-swipe-item>
  <mt-swipe-item><a href="javascript:void(0)">
          <img src="../assets/images/lb4.jpg" alt="">
      </a></mt-swipe-item>
  <mt-swipe-item><a href="javascript:void(0)">
          <img src="../assets/images/lb5.jpg" alt="">
      </a></mt-swipe-item>
</mt-swipe>
<section>
    <ul>
        <li><a href="javascript:void(0)">
            <img src="../assets/images/zq1.png" alt="">
            </a></li>
        <li><a href="javascript:void(0)">
            <img src="../assets/images/zq2.png" alt="">
            </a></li>
        <li><a href="javascript:void(0)">
            <img src="../assets/images/zq3.png" alt="">
            </a></li>
        <li><a href="javascript:void(0)">
            <img src="../assets/images/zq4.png" alt="">
            </a></li>
        <li><a href="javascript:void(0)">
            <img src="../assets/images/zq5.png" alt="">
            </a></li>
    </ul>
</section>
    </div>
</template>
<script>
export default {
  name: "SwipComponent"
};
</script>
<style scoped>
.mint-swipe {
  height: 110px;
}
.swiper .mint-swipe-item a img {
  width: 100%;
  height: 110px;
  /* vertical-align: top; */
}
ul {
  list-style: none;
  display: flex;
  width: 100%;
  overflow: hidden;
}
ul li {
  width: 20%;
}
ul li img{
    width: 75px;
    height: 76.8px;
}
.mint-swipe  {
  width: 100%;
  /* margin-left: 0px; */
  margin-top: 12px;
  overflow: hidden;
}
</style>


