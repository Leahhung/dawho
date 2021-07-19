<template>
  <div id="app">
    <navBar/>
    <Main/>
    <rightSide/>
  </div>
</template>

<script>
import Main from './components/main.vue'
import navBar from './components/navbar.vue'
import rightSide from './components/rightside.vue'
import $ from "jquery";

export default {
  name: 'App',
  components: {
    Main,
    navBar,
    rightSide
  }
}
</script>

<style lang="scss">
  @import "/src/assets/all.scss"
</style>
