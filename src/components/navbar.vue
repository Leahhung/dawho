<template>
  <div id="navbar">
    <div class="logo">
      <a href="https://dawho.tw/"><img src="https://dawho.tw/img/logo.svg"></a>
    </div>
    <div class="nav-items">
      <div class="nav-text">
      <ul>
        <li><a href="#">什麼是DAWHO</a></li>
        <li><a href="#">如何當DAWHO</a></li>
        <li><a href="#">DA熱門</a></li>
        <li><a href="#">FAQ</a></li>
      </ul>
      </div>
      <div class="nav-btn">
        <span class="btn btn-y">我要當DAWHO</span>
        <span class="btn btn-wb">進度查詢</span>
        <span class="btn btn-wb">立即下載</span>
      </div>
    </div>
    <div class="nav-ham" @click="giveMeCross"><span></span></div>
  </div>
</template>

<script>
export default {
  methods: {
    giveMeCross () {
      const hamBtn = document.querySelector('.nav-ham')
      const navItems = document.querySelector('.nav-items')
      // hamBtn.classList.toggle('is-change')
      if (navItems.style.transform === 'translateX(-110%)') {
        navItems.style.transform = 'translateX(0%)'
        hamBtn.classList.add('is-change')
      } else {
        navItems.style.transform = 'translateX(-110%)'
        hamBtn.classList.remove('is-change')
      }
    }
    // giveMeBurger () {
    //   const hamBtn = document.querySelector('.nav-ham')
    //   const navItem = document.querySelector('.nav-items')
    //   if (hamBtn.classList.contains('is-change')) {
    //     navItem.style.transform = 'translate(0%)'
    //   } else {
    //     navItem.style.transform = 'translate(-110%)'
    //   }
    // }
  }
}
</script>
