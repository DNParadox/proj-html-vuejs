<template>
  <div id="app">
    <MyHeader/>
  </div>
</template>

<script>
import MyHeader from './components/myHeader.vue'

export default {
  name: 'App',
  components: {
    MyHeader
}
}
</script>

<style lang="scss">
@import 'bootstrap';
@import './style/common.scss';
</style>
