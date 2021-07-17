<template>
  <div id="app">
    <navBar/>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <rightSide/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import navBar from './components/navbar.vue'
import rightSide from './components/rightside.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    navBar,
    rightSide
  }
}
</script>

<style lang="scss">
  @import "/src/assets/all.scss"
</style>
