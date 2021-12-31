<template>
  <div>
    <h1>首页页面</h1>
    <nuxt-link to="index">首页</nuxt-link>
    <a href="/">首页</a>
    <a href="/about">关于</a>
    <a href="/news">新闻</a>
    <!-- 这种配置比a更快加载，且不刷新 -->
    <nuxt-link :to="{name:'news',params:{newsId:3306,title:'切换标题',}}">news</nuxt-link>
    <nuxt-link :to="{name:'about'}">about</nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
