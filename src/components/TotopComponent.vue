<template>
  <div>
    <div class="back-top small" @click="backtop()" id="backtop">
        <img src="../assets/images/go-top.png" alt="">
    </div>
  </div>
</template>

<script>
  export default {
    // data() {
    //   return {
    //     backTopShow:false
    //   }
    // },
    // components: {},
    // mounted() {
    //   window.addEventListener('scroll', this.handleScroll)
    // },
    // methods: {
    //   backTop() {
    //     let back = setInterval(() => {
    //       if(document.body.scrollTop||document.documentElement.scrollTop){
    //         document.body.scrollTop-=200;
            
    //         document.documentElement.scrollTop-=200;
    //       }else {
    //         clearInterval(back)
    //       }
    //     });
    //   },
    //   handleScroll(){
    //     if (document.documentElement.scrollTop + document.body.scrollTop > 1500) {
    //       this.backTopShow=true;
    //     }
    //     else {
    //       this.backTopShow=false;
    //     }
    //   }
    // }

     mounted() {
    this.$(document).scroll(this.isShow);
  },
  methods: {
    isShow() {
      this.$(document).scrollTop() > 1020
        ? this.$("#backtop").removeClass("hidden")
        : this.$("#backtop").addClass("hidden");
    },
    backtop() {
      this.$("html").animate({
        scrollTop: 0
      });
    }
  }
  }
</script>

<style scoped>
  .back-top {
    position: fixed;
    right: 0.7rem;
    bottom: 3rem;
    width: 2.5rem;
    height: 2.5rem;
  }
  img{
    /* width: 2.5rem;
    height: 2.5rem; */
    width: 100%;
    height: 100%;
  }
  .hidden{
      display: none;
  }
</style>