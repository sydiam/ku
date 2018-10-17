<template>
 <div id="app">
     <!--图片轮播-->
     <!--练习:11:55 加载4张图片轮播显示-->
     <mt-swipe :auto="4000">
        <mt-swipe-item v-for="item in list">
          <img :src="item">
        </mt-swipe-item>
     </mt-swipe>
   </div>
</template>

<script>
     new Vue({
          el:"#app",
          data:function(){
            return {
              msg:"ok",
              list:[
              "img/banner1.png",
              "img/banner2.png",
              "img/banner3.png",
              "img/banner4.png"]
            }
          },
          methods:{
             show(){
               console.log("show()");
             }
          }
        })
</script>

<style>
    
</style>