<template>
  <div>
    用户端id
    <p>服务端或者路由切换时才执行</p>
    <div v-for="item in list">
      {{item.age + "*****" + item.num}}
    </div>
    <p>当前页面的数据1</p>
    <div>{{today}}</div>
  </div>
</template>

<script>
export default {
  async asyncData ({$axios}) {
    console.log($axios)
    let data = await $axios.post('/api/123/post',{value:1})
    return {
      list: data.data
    }
  },
  mounted(){
    this.today = '星期一'
  },
  data () {
    return {
      today: '星期五'
    }
  }
}
</script>

<style>

</style>
