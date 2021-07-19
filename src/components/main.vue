<template>
  <div id="mainpage">
    <header>
      <div class="slogan">
        <img src="../assets/logo-main.png" alt="">
        <span>新世代VIP數位帳戶</span>
      </div>
      <div class="middle">
        <div><span class="dollar-sign">💲</span><span class="middle-text">新台幣活儲最高利率</span><span class="middle-percent">1.1%</span></div>
        <div><span class="dollar-sign">💲</span><span class="middle-text">信用卡現金回饋最高</span><span class="middle-percent">8%</span></div>
      </div>
      <span class="header-btn">我要當DAWHO</span>
    </header>
    <main>
      <div class="item1">
        <img src="../assets/kv_01_img.jpeg" alt="">
        <div class="item1-right">
          <p class="l">養大<span class="red-l">你</span>的小錢</p>
          <p class="s">不只存錢同步養錢  小資也能成DAWHO</p>
          <p class="m">新台幣活儲最高利率<span class="percent">1.1%</span></p>
          <p class="xs">新台幣50萬元以內</p>
          <p class="item1-btn btn">了解更多＞</p>
        </div>
      </div>
      <div class="item2">
        <div class="item2-left">
          <p class="l">做自己的<span class="red-l">卡</span>神</p>
          <p class="s">刷卡消費變存款</p>
          <p class="xs">一般消費最高</p>
          <p class="m">國內<span class="percent">2%</span>國外<span class="percent">3%</span></p>
          <p class="red-s"><span class="red-dollar">💲</span>1%加碼現金回饋</p>
          <p class="ms">大戶等級上限1,500元/每月帳單</p>
          <p class="ms">大大等級上限300元/每月帳單</p>
          <p class="xs">專屬優惠加碼</p>
          <p class="m">國內<span class="percent">7%</span>國外<span class="percent">8%</span></p>
          <p class="red-s"><span class="red-dollar">💲</span>旅遊、外送、打Game通通加碼5%</p>
          <p class="ms">大戶等級上限600元/每月帳單</p>
          <p class="ms">大大等級上限300元/每月帳單</p>
          <p class="item2-btn btn">了解更多＞</p>
        </div>
        <img src="../assets/kv_02_img.jpeg" alt="">
      </div>
      <div class="item3"></div>
      <div class="item4"></div>
      <div class="item5"></div>
    </main>
    <footer>
      <div class="footer up">
        <p>千呼萬喚，質感上市</p>
        <div class="footer-main">
          <img src="../assets/footer_download.png" alt="">
          <p>三大特色功能搶先體驗</p>
          <p>帳務利息，天天更新 ｜ 消費回饋，輕鬆查詢 ｜ 安全簡易，無碼轉帳</p>
          <div>
            <img src="../assets/download_qrcode.png" alt="">
            <div class="download_content">
              <p>立即下載DAWHO</p>
              <p>最新版本號：iOS、Android 6</p>
              <p>最低支援作業系統：iOS 11.0(含)以上、Android 5.0(含)以上</p>
            </div>
          </div>
        </div>
      </div>
      <div class="footer down">
        <div class="down-left">謹慎理財 信用至上</div>
        <div>
          <p>24小時服務專線：(02)2528-7776/0800-058-888 (限市話)</p>
          <p>循環信用利率年息2.74%~15% (基準日2015/8/3)，預借現金手續費：預借現金金額X3.5%+指定金額</p>
          <p>(100元新台幣/3.5美元/350日圓/3歐元) 其他費用請上永豐銀行網站查詢</p>
        </div>
        <div>
          <p>©版權所有  <img src="../assets/footer_logo1.jpg" alt="">永豐銀行</p>
          <p><img src="../assets/footer_logo2.jpg" alt="">存款人存保權益 法定公告事項 隱私權保護聲明</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return{
      text: '123'
    }
  },
  methods: {
    counters() {
      const counters = document.querySelector('.counter');
      counters.forEach(function(counter) {
        counter.innerText = '0';
        const updateCounter = function() {
          const target = +counter.getAttribute('data-targett');
          const c = +counter.innerText;
          const increment = target / 200;
          if(c < target) {
            counter.innerText = `${Math.ceil(c + increment)}`;
            setTimeout(updateCounter, 0.1)
          } else {
            counter.innerText = target
          }
        }
      });
    }
  },
  created() {
    this.counters()
  },
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
