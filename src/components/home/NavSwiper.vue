<script setup>

import {ArrowRight} from "@element-plus/icons-vue";
</script>

<template>
 <div class="nav-swiper">
   <div class="nav-swiper-main">
     <div class="swiper-t">
       <ul>
         <li class="active">
           <span>HTML/CSS</span>
           <el-icon><ArrowRight/></el-icon>
         </li>
         <li>
           <span>HTML/CSS</span>
           <el-icon><ArrowRight/></el-icon>
         </li>
         <li>
           <span>HTML/CSS</span>
           <el-icon><ArrowRight/></el-icon>
         </li>
         <li>
           <span>HTML/CSS</span>
           <el-icon><ArrowRight/></el-icon>
         </li>
         <li>
           <span>HTML/CSS</span>
           <el-icon><ArrowRight/></el-icon>
         </li>
       </ul>
       <div>
         <el-carousel :interval="5000" arrow="always">
           <el-carousel-item v-for="item in 4" :key="item">
             <h3>{{ item }}</h3>
           </el-carousel-item>
         </el-carousel>
       </div>
     </div>
     <ul class="swiper-b">
       <li>
         <h3>
           <img src=""/>
         </h3>
         <div>
           <h4>初级课程</h4>
           <span>入门快，岗位多</span>
         </div>
       </li>
       <li>
         <h3>
           <img src=""/>
         </h3>
         <div>
           <h4>初级课程</h4>
           <span>入门快，岗位多</span>
         </div>
       </li>
       <li>
         <h3>
           <img src=""/>
         </h3>
         <div>
           <h4>初级课程</h4>
           <span>入门快，岗位多</span>
         </div>
       </li>
       <li>
         <h3>
           <img src=""/>
         </h3>
         <div>
           <h4>初级课程</h4>
           <span>入门快，岗位多</span>
         </div>
       </li>
       <li>
         <h3>
           <img src=""/>
         </h3>
         <div>
           <h4>初级课程</h4>
           <span>入门快，岗位多</span>
         </div>
       </li>
     </ul>

   </div>

 </div>
</template>

<style scoped>
.nav-swiper{
  display: flex;
  background: url("@/assets/img/微信图片_20240718170542.jpg");
  width: 100%;
  height: 600px;
}
.nav-swiper-main{
  width: 1000px;
  padding:47px 0;
  margin: 0 auto;
  color: #3585FF;
}

.swiper-t{
  display: flex;
  height: 373px;
  border-radius: 11px 11px 0px 0px;
}

.swiper-t ul{
  display: flex;
  flex-direction: column;
  width: 160px;
  height: 100%;
  justify-content: space-around;
  background: #2B283D;
  border-radius: 11px 0px 0px 0px;

}

.swiper-t ul li{
  display: flex;
  align-items: center;
  justify-content: space-around;
  width: 160px;
  height: 37px;
  font-size: 16px;
  color: #F2F2F2;
  cursor: pointer;
}
.active{

}
.swiper-t > div{
  width: 840px;
  height: 373px;
}
.el-carousel {
  line-height: 373px;
}

:deep .el-carousel_container{
  line-height: 373px;
}
.swiper-b{
  display: flex;
  //width: 100%;
}

.swiper-b li{
  display: flex;
  align-items: center;
  justify-content: center;
  width: 213px;
  height: 133px;
  cursor: pointer;
  background: #FFFFFF;
  border-radius: 0px 0px 0px 11px;

}
.swiper-b li img{
  width: 64px;
  height: 64px;
}
.swiper-b li div{
  margin-left: 11px;
}

.swiper-b li div h4{
  font-size: 16px;
  color: #333333;
}
.swiper-b li div span{
  font-size: 12px;
  color: #808080;
}
</style>