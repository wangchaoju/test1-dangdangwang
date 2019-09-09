<template>
    <div class="pinpai">
        <div class="jianju">

        </div>
       
        <div class="pp-list">
             <div class="pp">
            <img src="../assets/images/pinpaijie.jpg" alt="">
        </div>
            <mt-swipe :auto="3000">
                <mt-swipe-item>
                    <ul class="list1 clearfix">
                        <li><a href="#"><img src="../assets/images/pp1.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp2.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp3.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp4.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp5.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp6.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp7.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp8.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp9.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp10.png" alt=""></a></li>
                    </ul>
  </mt-swipe-item>
  <mt-swipe-item>   <ul class="list1">
                        <li><a href="#"><img src="../assets/images/pp11.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp12.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp13.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp14.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp15.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp6.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp7.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp8.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp9.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp20.png" alt=""></a></li>
                    </ul></mt-swipe-item>
  <mt-swipe-item>   <ul class="list1">
                        <li><a href="#"><img src="../assets/images/pp21.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp22.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp3.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp4.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp5.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp6.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp7.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp8.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp9.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/images/pp30.png" alt=""></a></li>
                    </ul></mt-swipe-item>
</mt-swipe>
        </div>
    </div>
</template>

<script>
export default {
  name: "PinpaiComponent"
};
</script>

<style scoped>
*{
    margin: 0;
    padding: 0;
}
.pp{
    height: 41.06px;
    /* overflow: hidden; */
    position: relative;
}
.pinpai {
  /* border: 1px solid red; */
  height: 196.06px;
  /* position: relative; */
}
.jianju {
  width: 100%;
  height: 5px;

  background-color: rgb(236, 232, 240);
}
.pp img {
  height: 41.06px;
  width: 100%;
}

.mint-swipe{
    width: 100%;
    height: 150px;
    /* display: flex;
    flex-direction: row;
    flex-wrap: wrap */
    /* position: relative; */
}
.mint-swipe .mint-swipe-item ul li a img{
  width: 75px;
  height: 75px;
}
.list1{
    width: 100%;
    height: 155px;
   display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    
}
.list1 li{
    width: 20%;
    list-style: none;
    height: 75px;
}

.mint-swipe .mint-swipe-indicator{
    background: blue;
}

</style>

