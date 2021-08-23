<template>
  <div id="app">
    <nav>
      <navBar/>
    </nav>
    <Main/>
    <rightSide/>
  </div>
</template>

<script>
import Main from './components/main.vue'
import navBar from './components/navbar.vue'
import rightSide from './components/rightside.vue'

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
@import "./src/assets/all.scss";
</style>
