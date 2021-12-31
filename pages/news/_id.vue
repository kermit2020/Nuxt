<template>
  <div>
    <h2>news_content</h2>
    <h2>动态路由页{{$route.params.id}}</h2>
    <nuxt-link to="/news">返回上一页</nuxt-link>
  </div>
</template>
<script>
export default {
  validate({params}) { //检验，如果失败则会返回404页面
    return /^\d+$/.test(params.id)
  },
  data() {
    return {
      title:this.$route.params.title
    }
  },
  head(){
    return {
      title:this.title,
      meta:[
        {hid:"description",name:"new副页",content:"这是一个news内容简介，便于SEO搜索"}
      ]
    }
  }
}
</script>