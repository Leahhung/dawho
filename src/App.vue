<template>
  <div id="app" :style="styleChange">
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
  },
  data() {
    return{
      styleChange: {
        height: '',
        width: ''
      }
    }
  },
  mounted() {
    const that = this;
    that.styleChange.height = document.body.clientHeight + "px";
    that.styleChange.width = document.body.clientWidth + "px";
  }
}
</script>

<style lang="scss">
  @import "/src/assets/all.scss"
</style>
