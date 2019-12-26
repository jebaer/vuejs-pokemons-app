<template>
  <div class="grey-background" id="app">
    <MyHeader></MyHeader>
  </div>
</template>

<script>
import MyHeader from './components/Header.vue'

export default {
  name: 'app',
  components: {
    MyHeader
  }
}
</script>

<style lang="sass">
#app
  font-family: 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50
  margin-top: "60px"
</style>
