<template>
    <div class="tushu">
        <div class="wph">
            <a href="#">
                <img src="../assets/images/close.jpg" alt="" class="manjian2">
            </a>
        </div>
           <div class="sx">
            <a href="#">
                <span>
                服装品牌榜单
                </span>
                <img src="../assets/images/icon-more1.png" alt="" class="icon-more">
            
            </a>
              <a href="#">
                <span>
                服装品牌单品
                </span>
                <img src="../assets/images/icon-more1.png" alt="" class="icon-more">
            
            </a>
               <a href="#">
                <span>
                服装馆
                </span>
                <img src="../assets/images/icon-more1.png" alt="" class="icon-more">
            
            </a>
            
        </div>
        <a href="#" class="ad1">
            <img src="../assets/images/manjian1.jpg" alt="" class="manjian">
        </a>

         <section class="part2">
            <a class="box" :href="item.href" v-for="(item, index) in items" :key="index">
                
                <img :src="item.img" alt="">
            </a>
        </section>
    </div>
</template>

<script>
import img1 from "../assets/images/clo1.jpg";
import img2 from "../assets/images/clo2.jpg";
import img3 from "../assets/images/clo9.jpg";
import img4 from "../assets/images/clo9.jpg";
import img5 from "../assets/images/clo8.jpg";
import img6 from "../assets/images/clo1.jpg";
import img7 from "../assets/images/clo7.jpg";
import img8 from "../assets/images/clo8.jpg";
import img9 from "../assets/images/clo9.jpg";
export default {
    data(){
        return {
        items:[ {state:"猫太子文具 ",price:"满100减50",img:img1,href:"https://www.sina.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img2,href:"https://www.sina.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img3,href:"https://www.sina.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img4,href:"https://www.baidu.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img5,href:"https://www.baidu.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img6,href:"https://www.baidu.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img7,href:"https://www.baidu.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img8,href:"https://www.baidu.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img9,href:"https://www.sina.com"},
               
            ]
        }
    }
}
</script>

<style scoped>
.jianju {
  width: 100%;
  height: 10px;

  background-color: rgb(236, 232, 240);
}
.jianju2 {
  width: 100%;
  height: 10px;
    margin-top: -4px;
  background-color: rgb(236, 232, 240);
}
.pic{
    width: 100%;
    /* height: 110.26px; */
    /* overflow: hidden; */
    /* border: 1px solid red; */
}
.ad1{
    display: block;
    height: 100.26px;

}
.manjian{
    width: 100%;
    height: 100.26px;
    margin-top: 10px;
}
.manjian2{
    width: 100%;
    height: 40.98px;
}
.sx{
    text-align: center;
    font-size: .5rem;
    height: 14.39px;
    margin-top: -5px;
}

.part2{
    margin-top: 15px;
}
    .part2 a img{
       width: 99%;
       height: 156.17px;
       /* margin: 0 auto; */
      
    }
    .box{
        display: inline-block;
        width: 33.33333%;
        height: 156.17px;
        text-align: center;
    }
</style>
