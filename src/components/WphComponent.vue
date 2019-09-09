<template>
    <div class="wph">
        <section class="part1">
            <ul >
                <li class="list1 clearfix">
                    <a href="#">
                        <img src="../assets/images/wph1.jpg" alt="">
                    </a>
                </li>
                <li class="list2 clearfix">
                    <p>探路者童装</p>
                    <b>满100减50</b>
                    <img src="../assets/images/wph2.jpg" alt="">
                </li>
                <li class="list3 clearfix">
                    <p>伊思Q</p>
                    
                    <b>低至49元</b>
                    <img src="../assets/images/wph3.jpg" alt="">
                </li>
            </ul>
        </section>
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
import img4 from "../assets/images/wph4.jpg";
import img5 from "../assets/images/wph5.jpg";
import img6 from "../assets/images/wph6.jpg";
import img7 from "../assets/images/wph7.jpg";
import img8 from "../assets/images/wph8.jpg";
import img9 from "../assets/images/wph9.jpg";
export default {
    data(){
        return {
            items:[
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
    .wph{
        width: 100%;
        overflow: hidden;
    }
    .list1,.list2,.list3{
        width: 33.33333%;
        height: 156.17px;
        text-align: center;
        position: absolute;
    }
    .list2{
        left: 33.33333%;
    }
    .list3{
        left: 66.66666%;
    }
    ul{
        margin-top: 10px;
        list-style: none;
        height: 156.17px;
        position: relative;
    }

    .list1 img{
        width: 100%;

    }
    .list2 img,.list3 img{
        width: 80%;
        height: 100px;
        position: absolute;
        bottom: 0;
        margin: 0 auto
    }
    .list2 img{
        left: 11.5px;
    }
    .list3 img{
        /* right: 0; */
        left: 11.5px;
    }
    p{
        font-size: 14px;
        padding-top: 15px;
    }
    b{
        font-size: 12px;
        color: #9b39e2
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

