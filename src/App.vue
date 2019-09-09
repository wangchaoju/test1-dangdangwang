<template>
  <div class="wrapper">
    <router-view/>

    <footer>
  
    </footer>
  </div>
</template>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
*{
  margin: 0;
  padding: 0;
}
html{
  font-size: 16px
}
body{
  padding-bottom: 46px;
}
a{
  text-decoration: none;
  color: #323232;
  
}
.icon-more{
  width: 12px;
  height: 12.38px;

}

.mint-swipe .mint-swipe-indicator.is-active {
    background: #f3344a;
}

.mint-swipe .mint-swipe-indicator {
    width: 4px;
    height: 4px;
    display: inline-block;
    border-radius: 100%;
    background: #000;
    opacity: 0.5;
    margin: 0 3px;
}
.mint-swipe .mint-swipe-indicators{
  bottom: 1px;
} 
.clearfix{
  clear: both;
}
</style>
