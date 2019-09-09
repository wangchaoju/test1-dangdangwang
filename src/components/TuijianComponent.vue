<template>
    <div class="tuijian">
        
        <div class="box">
            <a :href="item.jump_url" class="list"  v-for="(item, index) in items" :key="index">
            <img :src="item.image_url" alt="" class="img">
            <section class="name">{{item.name}}</section>
            <p>
                <span v-for="(item1, i) in item.productTags" :key="i">{{item1.name}}</span>
                
            </p>
            <span class="price">￥{{item.price}}</span>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    
    data(){
        return {
            items:[]
        }
    },
  created() {
    this.getData();
  },
  methods: {
    getData() {
      var vm = this;
      vm.axios
        .get(
          "/api/h5ajax.php?action=home&img_size=h&perm_id=20180709140948526139977800000953547"
        )
        .then(res => {
            this.items=res.data.reco_list
          console.log(res.data.reco_list);
        });
    }
  }
};
</script>

<style scoped>

p{
    text-align: left;
    padding-left: .3rem;
  
}
p span{
    padding: 0 .2rem;
}
p span:nth-of-type(1){
    border: 1px solid red;
    color: #f2303c;
    font-size: .418rem
}
p span:nth-of-type(2){
    background-color: #f2303c;
    color: #ffffff;
    font-size: .5rem;
    margin: 0 3px;
}
p span:nth-of-type(3){
    background-color: #f2303c;
    color: #ffffff;
    font-size: .5rem
}
.price{
    display: block;
    text-align: left;
    color: #f2303c;
    font-size: .6rem
}
.box{
    text-align: center;
    width: 100%;
    overflow: hidden;
    display: inline-block;
    /* background-color: #fff; */
}
.list{
    display: inline-block;
   
    width: 49.3%;
    padding-bottom: .4167rem;
    
}
/* .list:nth-of-type(2n){
    
    padding-left: .1042rem;
}
.list:nth-of-type(2n+1){
    padding-left: 0;   
    padding-right: .1042rem;
} */
.img{
    width: 11.5625rem;
    height: 11.5625rem;
}
.name{
   /* background-color: #fff; */
   text-align: left;
    font-size: .5417rem;
    overflow: hidden;
    line-height: .65remrem;
    height: 2rem;
    padding: 0 .2083rem;
}
.tuijian{
    /* background-color: rgb(239 244 250); */
    box-sizing: border-box
}
</style>