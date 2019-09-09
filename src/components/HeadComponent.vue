<template>
  <div class="header">
    <div class="logo clearfix">
      <img src="../assets/images/dd-logo1.png" alt="" class="logo" @click="home()">
    </div>
    <div class="search">
      <input type="text" placeholder="精选图书,没满100减40" class="search1">
      <img src="../assets/images/搜索.png" alt="" class="sousuo">
    </div>
    <div class="fenlei clearfix">
      <img src="../assets/images/分类.png" alt="" class="classify" @click="goList()">
    </div>
  </div>
</template>

<script>
export default {
  name: "HeadComponent",
  methods: {
    home() {},
    goList() {
      this.$router.push({ path: "/List" });
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  height: 30px;
  /* display: inline; */
  margin: 0;
  padding: 0;
}
.logo {
  float: left;
  margin-top: 1.5px;
  margin-left: 5px;
}
.search {
}
.search1 {
  outline: none;
  border: none;
  background-color: rgb(236, 232, 240);
  height: 28px;
  border-radius: 48px;
  /* width: 100% - 52px - 52px; */
  width: 65%;
  margin-left: 1rem;
  position: relative;
  padding-left: 30px;
  margin-top: 5px;
}

.sousuo {
  position: absolute;
  top: 7px;
  left: 60px;
  width: 25px;
  height: 25px;
  color: blue;
  opacity: 0.5;
}
.fenlei {
  float: right;
  display: inline-block;
  margin-top: -30px;
  margin-right: 7px;
}
.classify {
  width: 25px;
  height: 25px;
  opacity: 0.5;
}
</style>
