<template>
  <div class="home">
    <!-- <img src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <head-component></head-component>
    <swip-component></swip-component>
    <cuxiao-component></cuxiao-component>
    <pinpai-component></pinpai-component>
    <miaosha-component></miaosha-component>
    <miaoshaa-component></miaoshaa-component>
    <ad-component></ad-component>
    <wph-component></wph-component>
    <tushu-component></tushu-component>
    <clo-component></clo-component>
    <super-component></super-component>
    <dianqi-component></dianqi-component>
    <totop-component></totop-component>
    <tuijian-component></tuijian-component>
    <footer-component></footer-component>
  </div>
</template>

<script>
// @ is an alias to /src
import HeadComponent from "@/components/HeadComponent.vue";
import SwipComponent from "@/components/SwipComponent.vue";
import CuxiaoComponent from "@/components/CuxiaoComponent.vue";
import PinpaiComponent from "@/components/PinpaiComponent.vue";
import MiaoshaComponent from "@/components/MiaoshaComponent.vue";
import FooterComponent from "@/components/FooterComponent.vue";
import MiaoshaaComponent from "@/components/MiaoshaaComponent.vue";
import AdComponent from "@/components/AdComponent.vue";
import WphComponent from "@/components/WphComponent.vue";
import CloComponent from "@/components/CloComponent.vue";
import TushuComponent from "@/components/TushuComponent.vue";
import SuperComponent from "@/components/SuperComponent.vue";
import DianqiComponent from "@/components/DianqiComponent.vue";
import TuijianComponent from "@/components/TuijianComponent.vue";
import TotopComponent from "@/components/TotopComponent.vue";
export default {
  name: "home",

  components: {
    HeadComponent,

    SwipComponent,
    CuxiaoComponent,
    PinpaiComponent,
    MiaoshaComponent,
    MiaoshaaComponent,
    AdComponent,
    FooterComponent,
    WphComponent,
    TushuComponent,
    CloComponent,
    SuperComponent,
    DianqiComponent,
    TuijianComponent,
    TotopComponent
  },
 
};
</script>

