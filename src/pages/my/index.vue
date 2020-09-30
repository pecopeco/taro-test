<template lang="pug">
view.my my
</template>

<script>
export default {
  name: 'my',
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

.my {
}
</style>