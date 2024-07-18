<template>
  <header>
    <div class="header-main">
      <div class="header-l">
        <h1 class="logo">
          <img src="@/assets/img/logo.png">
        </h1>
        <ul>
          <li class="active">首页</li>
          <li>课程</li>
          <li>会员</li>
        </ul>
      </div>
      <div class="header-r">
        <div class="search">

          <input type="text" placeholder="搜索想要的课程">
          <el-icon color="F0F2F4" size="20"><Search/></el-icon>
        </div>
        <div class="shop">
          <el-icon color="F0F2F4" size="20"><ShoppingCart/></el-icon>
          <i></i>
        </div>
        <div class="login">
          登录/注册
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import {
  Search,
  ShoppingCart,
} from '@element-plus/icons-vue';
import { ElButton } from 'element-plus'
import 'element-plus/dist/index.css';

const components = {
  ElButton,
};
</script>

<style scoped>
header {
  width: 100%;
  height: 80px;
}
.header-main {
  justify-content: space-between;
  align-items: center;
  display: flex;
  width: 1000px;
  height: 80px;
  margin: 0 auto;
}
.header-l {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.active{
  position:relative;
  color: #3585FF;
  font-family: Microsoft YaHei;
}
.active:after{
  content:"";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 120%;
  height: 2px;
  background-color: #3585FF;
  margin-left: -20%;
}
.logo {
  width: 127px;
  height: 50px;
  margin-right: 51px;
}
.header-l ul {
  display: flex;
  height: 50px;
}
.header-l ul li{
  line-height: 50px;
  font-weight: 500;
  cursor: pointer;
}
.header-l ul li + li{
  margin-left: 79px;
  font-size: 16px;
  color: #808080;

}
.header-r {
  display: flex;
  align-items: center;
}
.header-r .search {
  display: flex;
  align-items: center;
  padding: 0 10px;
  width: 300px;
  height: 43px;
  background: #F0F2F4;
  border-radius: 5px;
}
.header-r .search input {
  width: 100%; /* 修改为100% */
  height: 43px;
  border: none;
  background: transparent;
}
.header-r .shop{
  margin-left: 42px;
  display: flex;
  align-items: center;
}
.header-r .login{
  margin-left: 0px;
  font-size: 16px;
  color: #808080;
  cursor: pointer;
}

</style>