<template>
    <div class="listbox">
        <div class="box">
<a href="#" v-for="(item,i) in items" :key="i">
                <span ><img :src="item.img" ></span>
                <span class="state">{{item.state}}</span>
                <span class="np">￥{{item.newprice}}</span>
                <span class="price">￥{{item.price}}</span>                        
            </a>
            <a href="#"><img src="../assets/images/mx11.png" alt=""></a>
            
        </div>
            
        </div>
</template>
<script>
import img1 from "../assets/images/mx1.jpg";
import img2 from "../assets/images/mx2.jpg";
import img3 from "../assets/images/mx3.jpg";
import img4 from "../assets/images/mx4.jpg";
import img5 from "../assets/images/mx5.jpg";
import img6 from "../assets/images/mx6.jpg";
import img7 from "../assets/images/mx7.jpg";
import img8 from "../assets/images/mx8.jpg";
import img9 from "../assets/images/mx9.jpg";
import img10 from "../assets/images/mx10.jpg";
export default {
      
  name: "MiaoshaaComponent",
  data() {
    return {
        items:[
            {img:img1,state:"美特斯邦威旗下4M短袖T恤2018夏季新款男基础百搭纯色短袖T恤",newprice:"29",price:"99.00"},
            {img:img2,state:"儿童长高食谱",newprice:"12.5",price:"29.80"},
            {img:img3,state:"凉生，我们可不可以不忧伤1 陌上郎（典藏版）（同名影视剧由钟汉良、马天宇、孙怡、于朦胧等联袂出演）",newprice:"17.8",price:"38.88"},
            {img:img4,state:"免邮 苹果X手机壳iPhone8/7防摔闪粉玻璃保护套6s plus简约小清新男女款 小猪社会猪手机套",newprice:"29",price:"99.00"},
            {img:img5,state:"【新疆特产】新疆特产库尔勒香梨 一级新鲜梨子孕妇水果5斤整箱包邮",newprice:"29.9",price:"99.00"},
            {img:img6,state:"熊本熊-13寸儿童书包呆萌可爱出行书包GZ0122",newprice:"49",price:"258.00"},
            {img:img7,state:"墨菲定律",newprice:"14.9",price:"48.00"},
            {img:img8,state:"AIRTEX亚特皮肤风衣登山旅行防晒抗紫外线透气钓鱼男女皮肤风衣",newprice:"69",price:"599.00"},
            {img:img9,state:"在重点高中等你（全4册）初中三年综合学力提升手册 全国初中名校联盟连续5年推荐",newprice:"49",price:"122.25"},
            {img:img10,state:"得力桶装原木铅笔2B/HB/2H铅笔50支 学生儿童写字绘画奖品",newprice:"17.5",price:"49.00"}
           
        ]
    };
  }
};
</script>
<style scoped>
*{
    margin: 0;
    padding: 0;
}
img{
    width: 96.02px;
    height: 96.02px;
}
a{
    text-decoration: none;
    color: rgb(153, 153, 153);
    width: 106.02px;
    height: 180px;
    display: inline-block;
    vertical-align: top;
    overflow: hidden;
    padding: 0 .21rem;

}
.listbox{
    margin-top: 22px;
    overflow: hidden;
    overflow-x:scroll;
    /* overflow-y: scroll; */
    
}   
   
.listbox::-webkit-scrollbar {display:none}
.box{
    width: 1250px;
    height: 180px;
}
span{
    display: block;
}
.state{
    font-size: .42rem;
    margin-top: .4rem;
    height: 29.39px;
    overflow: hidden;
    text-align: left;
}
.np{
    font-size: 16px;
    color: #f3344a;
}
.price{
    color: #bababa;
    text-decoration: line-through;
    font-size: 12px
}

</style>


