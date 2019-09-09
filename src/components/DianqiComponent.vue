<template>
    <div class="super">
        <div class="jianju">

        </div>
     <div class="wph">
            <a href="#">
                <img src="../assets/images/dianqicheng.jpg" alt="" class="manjian2">
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
             <a href="#">
                <span>
                网络文学
                </span>
                <img src="../assets/images/icon-more1.png" alt="" class="icon-more">
            
            </a>
        </div>
        <a href="#" class="ad1">
            <img src="../assets/images/dianqi1.jpg" alt="" class="manjian">
        </a>
      <div class="box2">
              <a class="no1 clearfix">
                <span class="part1">
                        <p >三只松鼠</p>
                        <b>满199减120</b>
                </span>
                <img class="pic1" src="../assets/images/super2.png" alt="">       
            </a>
        
            <a class="no4">
                    <span class="part2">
                            <p>三只松鼠</p>
                            <b>满199减120</b>
                    </span>
                    <img class="pic2" src="../assets/images/super2.png" alt="">    
            </a>
        </div>

         <section class="part4">
            <a class="box4" :href="item.href" v-for="(item, index) in items" :key="index">
                <p class="p1">{{item.state}}</p>
                <b class="b1">{{item.price}}</b>
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
export default {
    data(){
        return {
        items:[ {state:"猫太子文具 ",price:"满100减50",img:img1,href:"https://www.sina.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img2,href:"https://www.sina.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img3,href:"https://www.sina.com"},
                {state:"猫太子文具 ",price:"满100减50",img:img4,href:"https://www.baidu.com"},
                              
            ]
        }
    }
}
</script>


<style scoped>
.jianju {
  width: 100%;
  height: 10px;
  margin-top: -4px;
  background-color: rgb(236, 232, 240);
}

.pic {
  width: 100%;
  /* height: 110.26px; */
  /* overflow: hidden; */
  /* border: 1px solid red; */
}
.ad1 {
  display: block;
  height: 100.26px;
}
.manjian {
  width: 100%;
  height: 100.26px;
  margin-top: 10px;
}
.manjian2 {
  height: 40.98px;
}
.sx {
  text-align: center;
  font-size: 0.5rem;
  height: 14.39px;
  margin-top: -5px;
}
.box {
   
  height: 172px;
  font-size: 12px;
}
.box a {
  display: inline-block;
}

.list1 {
  width: 50%;
  height: 172px;
  float: left;
}
.list2,
.list3 {
  float: right;
  width: 50%;
  height: 86px;
  overflow: hidden;
}
.list1 img {
  width: 121px;
  height: 121px;
  margin-left: 50px;
  margin-top: 10px;
}
.list2 img,
.list3 img {
  width: 79px;
  height: 79px;
  margin-left: 100px;
  margin-top: -30px;
  /* margin-top: 30px; */
}
a{
    display: inline-block;
}

.no1,
        .no2 {
            width: 187.5px;
            height: 86px;
            float: right;
            /* margin: 2px; */
            /* border: 1px solid red; */
            position: relative;
        }

        .no2,.no1{
            clear: both
        }

        .no3 {
            /* margin-left: 110px; */
            width: 187.5px;
            height: 172px;
            /* border: 1px solid blue; */
            position: relative;
        }
        .pic1,.pic2{
            width: 79px;
            height: 79px;
            top: 5px;
            right: 2px;
            position: absolute;
        }
        .pic3{
            width: 110px;
            height: 110px;
            position: absolute;
            top: 60px;
            right: 5px;
        }
       
        p{
            height: 19px;
            font-size: 14px;
            margin: 0;
        }
        b{
            font-weight: normal;
            color: dodgerblue;
            font-size: 12px
        }
        .part3{
            position: absolute;
            top: 5px;
            left: 10px;

        }
        .part1,.part2{
            position: absolute;
            top: 25px;
            left: 10px;
        }
         .no4{
           /* clear: both; */
            float: right;
            width: 187.5px;
            height: 86px;
            position: relative;
        }
        .box2{
            margin-top: 15px;
            height: 86px;
            clear: both;
        }


         .p1{
        font-size: 14px;
        padding-top: 15px;
        font-weight: normal;
    }
    .b1{
        font-size: 12px;
        font-weight: normal;
        color: dodgerblue;
    }

    .part4 a img{
       width: 75px;
       height: 75px;
       /* margin: 0 auto; */
      
    }
    .box4{
        display: inline-block;
        width: 93.75px;
        height: 127px;
        text-align: center;
    }
</style>
