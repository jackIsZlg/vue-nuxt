<template>
  <section>
    <div class="main">
      <h2>主页</h2>
      <h3>当前计数{{$store.state.counter}}</h3>
    </div>
    <nuxt-link to="/user/1">去用户页面</nuxt-link>
  </section>
</template>

<script>

export default {
  asyncData ({req}) {
      if(req){
        console.error(req.headers.cookie)
      }
     return {}
  },
  components: {

  },
  created () {
    // this.$axios.get('/api/123/get', {
    // }).then(function (res) {
    //
    // }).catch(function (err) {
    //   console.log(err)
    // })
  },
  data () {
    return {

    }
  },
  methods: {

  },
  head () {
    return {
      title: '小册',
      meta: [
        { hid: 'events custom title', name: 'events', content: 'events custom title description' }
      ]
    }
  },
}
</script>

<style scoped lang="less">
  .main {
    font-size: 14px;
  }

</style>
