<template>
  <div class="list">
    <div class="listItem" v-for="(item, index) in list" :key="index">
      {{ item.name }}
    </div>
    <van-button type="primary">主要按钮</van-button>
<van-button type="info">信息按钮</van-button>
<van-button type="default">默认按钮</van-button>
<van-button type="warning">警告按钮</van-button>
<van-button type="danger">危险按钮</van-button>
  </div>
</template>

<script>
import Vue from 'vue'
import { Button } from 'vant'
Vue.use(Button)
export default {
  data () {
    return {
      list: [
        { name: 'vue-cli4脚手架' },
        { name: 'vant按需引入' },
        { name: '移动端rem适配' },
        { name: 'axios拦截封装' },
        { name: 'util工具类函数封装' },
        { name: 'vue-router配置' },
        { name: '登录权限校验' },
        { name: '多环境变量配置' },
        { name: 'vue.config.js配置' },
        { name: 'toast组件封装' },
        { name: 'dialog组件封装' },
        { name: '跨域代理设置' },
        { name: 'webpack打包可视化分析' },
        { name: 'CDN资源优化' },
        { name: 'gzip打包优化' },
        { name: '首页添加骨架屏' },
        { name: '首页添加骨架屏' },
        { name: '使用SvgIcon 组件' }
      ]
    }
  }
}
</script>

<style scoped lang="less">
.list {
  height: 100%;
  width: 100%;
  .listItem {
    width: 100%;
    padding: 0 15px;
    height: 45px;
    line-height: 45px;
    position: relative;
    background-color: #fff;
    border-bottom: 1px solid #ddd;
    text-align: left;
  }
}
</style>
