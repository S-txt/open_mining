<template>
<header id="header" class="header">
  <img src="../src/assets/Logo.svg" alt="" class="logo">
  <ul class="menu">
    <li>
      <a href="#">О проекте</a>
    </li>
    <li>
      <a href="#">Тарифы</a>
    </li>
    <li>
      <a href="#">FAQ</a>
    </li>
    <li>
      <a href="#">Контакты</a>
    </li>
    <li class="login">
      <a href="#">Вход</a>
    </li>
  </ul>
</header>
<div class="main">
  <div class="main_container">
    <h1>
      Снижение рисков связанных с майнингом по максимуму
    </h1>
    <h6>
      Честность майнинга заложена в архитектуре
    </h6>
    <ul>
      <li>
        <a href="#" class="btn" id="btn_1">Начать зарабатывать</a>
      </li>
      <li>
        <a href="#" class="btn" id="btn_2">Узнать больше</a>
      </li>
    </ul>
  </div>
</div>
<div class="about">
  <img id="laptop" src="../src/assets/img/Laptop.png">
</div>
  
</template>

<script>
export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-BoldItalic.ttf') format('truetype');
  font-weight: bold;
  font-style: italic;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-Italic.ttf') format('truetype');
  font-weight: normal;
  font-style: italic;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-Medium.ttf') format('truetype');
  font-weight: 500;
  font-style: normal;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-BlackItalic.ttf') format('truetype');
  font-weight: 900;
  font-style: italic;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-Bold.ttf') format('truetype');
  font-weight: bold;
  font-style: normal;
}

@font-face {
  font-family: 'Gotham Pro Narrow';
  src: url('assets/Fonts/GothamProNarrow-Bold.ttf') format('truetype');
  font-weight: bold;
  font-style: normal;
}

@font-face {
  font-family: 'Gotham Pro Narrow';
  src: url('assets/Fonts/GothamProNarrow-Medium.ttf') format('truetype');
  font-weight: 500;
  font-style: normal;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-LightItalic.ttf') format('truetype');
  font-weight: 300;
  font-style: italic;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-Light.ttf') format('truetype');
  font-weight: 300;
  font-style: normal;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-Black.ttf') format('truetype');
  font-weight: 900;
  font-style: normal;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'Gotham Pro';
  src: url('assets/Fonts/GothamPro-MediumItalic.ttf') format('truetype');
  font-weight: 500;
  font-style: italic;
}
body{
  margin: 0;
}
*{
  font-family: 'Gotham Pro', sans-serif;
  text-decoration: none;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;

  margin: 0;
}
template{
  width: 1920px;
}
header{
  width: 100%;
  display: flex;
  align-items: center;
  margin-top: 48px;
  font-size: 24px;
  line-height: 130%;
}
.logo{
  height: 72px;
}
li{
  list-style: none;
}
header a{
  color: black;
}
.menu{
  display: flex;
  justify-content: center;
}
.menu li a {
  text-decoration: none;
  font-size: 16px;
  margin-left: 1em;
}
.graph{
  position: relative;
  opacity: 30%;
  object-fit: scale-down;
  overflow:hidden;
  width: 100%;
  z-index: 0;
}
#graph_2{
  margin-top: -13%;
}
h1{
  font-size: 60px;
  line-height: 130%;
  letter-spacing: 2px;
  font-weight: 700;
}
h6{
  font-size: 24px;
  line-height: 130%;
  font-weight: 400;
}
.main_container {
  width: 840px;
  margin: 0 auto;
  padding: 0 10% 100px 10%;
}
.main_container::after{
  position: absolute;
  content:"";
  width: 100%;
  height: 100%;
  top: 170px;
  left: 0;
  opacity: 0.15;
  z-index: -1;
  background:
      url("../src/assets/bg/graph_1.svg")  no-repeat,
      url("../src/assets/bg/graph_2.svg") 0 140px no-repeat;
}
.main_container ul{
  display: flex;
  justify-content: center;
  margin-top: 3px;
}
.main_container a{
  margin:27px;
}
.btn{
  padding: 14px 18px;
  border-radius: 4px;
}
#btn_1{
  background-color: #87B645;
  color: white;
  transition: 0.3s ease;
}
#btn_2{
  border: 1px solid #A0C4FA;
  color: #333333;
  font-weight: 300;
  transition: 0.3s ease;
}
#btn_2:hover{
  border: 1px solid #FBAC00;
  color: white;
  background: #FBAC00;
}
#btn_2:active{
  border: 1px solid #2B69DD;
  background: #2B69DD;
  color: #75ACFE;
}
#btn_2:disabled{
  border: 1px solid #D7D7D7;
  color: #D7D7D7;
}
.about{
  overflow-y: hidden;
  background-image: url("../src/assets/bg/spot1.png");
  background-repeat: no-repeat;
  background-position: right;
}

.bg {
  position: absolute;
  z-index: 0;
  overflow: hidden;
}
#spot1{
  position: absolute;
  left: 1070px;
  overflow: hidden;
  z-index: -1;

}
#laptop{
  margin: 0 auto;
}

</style>
