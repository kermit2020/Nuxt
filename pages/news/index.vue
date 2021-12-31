<template>
  <div name="index">
    <h2>新闻页面</h2>
    <marquee behavior="" direction="left"> news,看见了吗新闻,newID:{{$route.params.newsId}}</marquee>
     <nuxt-link :to="{name:'index'}">返回首页</nuxt-link>
     <ul>
       <li><a href="/news/123">new-1</a></li>
       <li><a href="/news/456">new-2</a></li>
       <li><a href="/news/dsfsdf">new-3</a></li>
       <li><nuxt-link :to="{name:'news-id',params:{id:789}}">new-4</nuxt-link></li>
     </ul>
  </div>
</template>
<script>
export default {
  transition:'text1'
}
</script>