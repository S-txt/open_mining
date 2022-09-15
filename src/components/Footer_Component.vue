<template>
<div class="footer_container">
  <img src="../assets/Logo.png">
  <ul class="footer">
    <li class="Text_2_24_Regular"><a href="#">О проекте</a></li>
    <li class="Text_Main_18_Regular"><a href="#">Вход</a></li>
    <li class="Text_Main_18_Regular"><a href="#">Регистрация</a></li>
    <li class="Text_2_24_Regular"><a href="#">Тарифы</a></li>
    <li class="Text_Main_18_Regular"><a href="#">Предложение</a></li>
    <li class="Text_Main_18_Regular"><a href="#">Оферта</a></li>
    <li class="Text_2_24_Regular"><a href="#">FAQ</a></li>
    <li class="Text_Main_18_Regular"><a href="#">Тарифы</a></li>
    <li class="Text_Main_18_Regular"><a href="#">Оплата</a></li>
    <li class="Text_2_24_Regular"><a href="#">Контакты</a></li>
    <li class="Text_Main_18_Regular"><a href="tel:8 800 920 00 00">8 800 920 00 00</a></li>
    <li class="Text_Main_18_Regular"><a href="mailto:honest@maning.ru">honest@maning.ru</a></li>
  </ul>
  <div class="social_media">
    <a class="facebook" href="#"/>
    <a class="instagram" href="#"/>
  </div>
</div>
  <span class="watermark">© 2019 Honest Mining</span>
</template>

<script>
export default {
  name: "Footer_Component"
}
</script>

<style scoped>
.footer_container{
  width: 100vw;
  height: 430px;
  background: url("../assets/bg/spot6.png") left bottom no-repeat,
              url("../assets/bg/spot7.png") right bottom no-repeat;
  display: flex;
  flex-flow: row;
  align-items: center;
  justify-content: space-around;
}

.footer{
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(3, auto);
  grid-auto-flow: column;
  gap: 32px;
  width: 800px;
  padding: 0;
}

.social_media{
  width: 160px;
  height: 56px;
  display: flex;
  flex-flow: row;
  justify-content: space-between;
}
.facebook{
  width: 56px;
  height: 56px;
  background: url("../assets/Icons/ic_facebook.png") center no-repeat;
  background-size: 12px 22px;
}
.instagram{
  width: 56px;
  height: 56px;
  background: url("../assets/Icons/ic_instagram.png") center no-repeat;
  background-size: 22px;
}
.watermark{
  position: relative;
  display: flex;
  align-items: center;
  text-align: center;
  font-weight: 400;
  font-size: 12px;
  line-height: 0;
  justify-content: center;
  color: #A1A1A3;
  bottom: 40px;
  margin-left:auto;
  z-index: 0;

}

@media screen and (max-width: 768px){
  .footer{
    display: none;
  }


}
</style>