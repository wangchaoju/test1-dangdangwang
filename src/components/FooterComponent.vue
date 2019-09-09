<template>
    <footer>
<mt-tabbar >
  <mt-tab-item id="首页">
    <img slot="icon" src="../assets/images/f1.png">
    
  </mt-tab-item>
  <mt-tab-item id="分类">
    <img slot="icon" src="../assets/images/f2.png" @click="goList()">
    
  </mt-tab-item>
  <mt-tab-item id="我的当当">
    <img slot="icon" src="../assets/images/f3.png">
    
  </mt-tab-item>
  <mt-tab-item id="购物车">
    <img slot="icon" src="../assets/images/f4.png">
    
  </mt-tab-item>
  <mt-tab-item id="下载">
    <img slot="icon" src="../assets/images/f5.png">
    
  </mt-tab-item>
</mt-tabbar>
    </footer>
</template>

<script>
export default {
  name: "FooterComponent",
  methods:{
    goList(){
      this.$router.push({path:'/List'})
    }
  }
};
</script>

<style scoped>
img{
    width: 35px;
    height: 35px;
   
}
.mt-tabbar .mt-tab-item{
  
  width: 20%;
}

.mint-tabbar{
  
  width: 100%;
  /* height: 46px; */
  overflow: hidden;
  position: fixed;
  bottom: 0px;
}
</style>


