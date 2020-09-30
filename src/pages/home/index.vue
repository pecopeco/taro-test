<template lang="pug">
view.home
  view.msg {{query}}
  button.btn(@tap="go({path: 'detail', query: {id: 1}})") go detail
</template>

<script>

export default {
  name: 'home',
  components: {
  },
  data() {
    return {
      query: 'vue 3'
    }
  },
  methods: {
    submit () {
      console.log('get')
    }
  },
  onShow () {
    console.log(this.query)
    this.submit()
  }
}
</script>

<style vars lang="stylus">

.home {
  .logo {
    width 100px
    height 100px
  }
  .msg {
    color theme
  }
}
</style>