<template>
    <div class="miaosha">
        <div class="jianju">

        </div>
        <div class="logo">
            <img src="../assets/images/miaosha.jpg" alt="">
            <a href="#" class="more">更多</a>
        </div>
        <div class="time">
            倒计时
        </div>
        
    </div>
</template>
<script>

export default {
  
};
</script>
<style scoped>
.jianju {
  width: 100%;
  height: 5px;

  background-color: rgb(236, 232, 240);
}
.miaosha {
  width: 100%;
  height: 80px;
  /* border: 1px solid red; */
  overflow: hidden;
}
.logo {
  position: relative;
  overflow: hidden;
}
.logo img {
  width: 100%;
  height: 41.06px;
}
.more {
  position: absolute;
  right: 5px;
  top: 10px;
  text-indent: -9999px;
}
.time {
  height: 25px;
  text-align: center;
  border: 1px solid red;
  margin-bottom: 22px;
}

</style>


