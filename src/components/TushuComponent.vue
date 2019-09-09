<template>
    <div class="tushu">
        <div class="wph">
            <a href="#">
                <img src="../assets/images/tushu.jpg" alt="" class="manjian2">
            </a>
        </div>
           <div class="sx">
            <a href="#">
                <span>
                当当书城
                </span>
                <img src="../assets/images/icon-more1.png" alt="" class="icon-more">
            
            </a>
              <a href="#">
                <span>
                电子书
                </span>
                <img src="../assets/images/icon-more1.png" alt="" class="icon-more">
            
            </a>
            
        </div>
        <a href="#" class="ad1">
            <img src="../assets/images/tushu1.jpg" alt="" class="manjian">
        </a>

         <section class="part2">
            <a class="box" :href="item.href" v-for="(item, index) in items" :key="index">
                <p>{{item.state}}</p>
                <b>{{item.price}}</b>
                <img :src="item.img" alt="">
            </a>
        </section>
    </div>
</template>

<script>
import img1 from "../assets/images/wph1.jpg";
import img2 from "../assets/images/wph2.jpg";
import img3 from "../assets/images/wph3.jpg";
import img4 from "../assets/images/wph4.jpg";
import img5 from "../assets/images/wph5.jpg";
import img6 from "../assets/images/wph6.jpg";
import img7 from "../assets/images/wph7.jpg";
import img8 from "../assets/images/wph8.jpg";
import img9 from "../assets/images/wph9.jpg";
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
    },

  
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
    display: inline-block;
    height: 100.26px;

}
.manjian{
    width: 100%;
    height: 100.26px;
    margin-top: 10px;
}
.manjian2{
    height: 40.98px;
}
.sx{
    text-align: center;
    font-size: .5rem;
    height: 14.39px;
    margin-top: -5px;
}



  p{
        font-size: 14px;
        padding-top: 15px;
    }
    b{
        font-size: 12px;
        color: #ef2933
    }

    .part2 a img{
       width: 80%;
       height: 100px;
       /* margin: 0 auto; */
      
    }
    .box{
        display: inline-block;
        width: 33.33333%;
        height: 156.17px;
        text-align: center;
    }
</style>
