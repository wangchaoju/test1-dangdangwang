<template>
    <div class="cuxiao">
     
        <div class="cx clearfix">
            <img src="../assets/images/cx.png" alt="">
        </div>
        <!-- <ul class="xx">
            <li><a href="#">
                <span class="hot">热卖</span>
                <span class="deta">竹炭狗公仔9.9包邮</span>
                </a></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
        </ul> -->
        <div id="box">
    <ul id="con1" ref="con1" :class="{anim:animate==true}">
      <!-- <span class="hot">热卖</span> -->
    <li v-for='(item,i) in items' :key=i><a href="#"><span class="hot">热卖</span>{{item.name}}</a></li>
      </ul>
</div>
        <div class="more">
            <a href="#">更多</a>
        </div>
    
    </div>
</template>

<script>
export default {
  // name:"CuxiaoComponent"
  data() {
    return {
      animate: false,
      items: [
        { name: "竹炭狗公仔9.9包邮" },
        { name: "30万图书，每满100减40" },
        { name: "蒲公英童书馆品牌日5折封顶" },
        { name: "中小学阅读，每满99减50" },
        { name: "外语考试图书，每满100减30" },
        { name: "创意文具满99减5" }
      ]
    };
  },
  created() {
    setInterval(this.scroll, 3000);
  },
  methods: {
    scroll() {
      this.animate = true; // 因为在消息向上滚动的时候需要添加css3过渡动画，所以这里需要设置true
      setTimeout(() => {
        //  这里直接使用了es6的箭头函数，省去了处理this指向偏移问题，代码也比之前简化了很多
        this.items.push(this.items[0]); // 将数组的第一个元素添加到数组的
        this.items.shift(); //删除数组的第一个元素
        this.animate = false; // margin-top 为0 的时候取消过渡动画，实现无缝滚动
      }, 5000);
    }
  }
};
</script>
<style scoped>
.cuxiao {
  height: 42px;
  position: relative;
}
.cx img {
  float: left;
  width: 80px;
  height: 42px;
  margin-left: 10px;
}
.xx {
  float: left;
  height: 42px;
  overflow: hidden;
}
ul li {
  height: 42px;
  line-height: 42px;
}

ul li a span {
  color: rgb(60, 60, 60);
  font-size: 0.55rem;
}
.more {
  width: 42px;
  height: 42px;
  line-height: 42px;
  float: right;
  font-size: 13px;
}
.more a {
  color: rgb(153, 153, 153);
}
.hot {
  font-size: 0.55rem;
  color: tomato;
  padding: 0px 3px;
  border: 1px solid tomato;
  margin-right: 7px;
  margin-left: 15px;
}



#box{
    width: 214px;
    /* margin-top: 5px; */
    padding-top: 18px;
    height: 24px;
    overflow: hidden;
    /* padding-left: 30px; */
    /* border: 1px solid black; */
    font-size: .55rem;
    position: absolute;
    left: 80px;
}
.anim{
    transition: all 1.2s;
    margin-top: -42px;
}
#con1 li{
    list-style: none;
    line-height: 8px;
    color: rgb(153, 153, 153);
}
#con1 li a{
  color: rgb(153, 153, 153);
}
</style>


