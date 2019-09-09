<template>
<div class="list">
  <List-component></List-component>
  页面开发中.....
  <router-link to='/'>aaaa</router-link>
</div>
    
</template>

<script>
import $ from 'jquery'
import ListComponent from "@/components/ListComponent.vue";
export default {
  name: "list",
  components: {
    ListComponent
  }
};
</script>
