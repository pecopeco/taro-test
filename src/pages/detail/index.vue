<template lang="pug">
view.detail detail
</template>

<script>
export default {
  name: 'detail',
  data() {
    return {
      query: '123'
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

.detail {
}
</style>