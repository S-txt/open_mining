<template>
  <div class="header">
    <img src="../../src/assets/Logo.svg" alt="" class="logo">
    <ul class="menu Text_2_24_Regular">
      <li>
        <a href="#" class="">О проекте</a>
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
    </ul>
    <div class="login_container">
      <div class="burger"/>
      <div class="login">
        <a href="#">Вход</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
name: "Header_Component"
}
</script>

<style scoped>
.header{
  width: 100vw;
  display: flex;
  align-items: center;
  margin-top: 48px;
  font-size: 24px;
  line-height: 130%;
  justify-content: space-around;
  overflow: hidden;
}
.logo{
  height: 72px;
}
.menu{
  display: flex;
  justify-content: space-around;
  width: 40%;
  align-items: center;
  padding: 0;
  overflow-x: clip;
  min-width: 500px;
}
.menu li a {
  margin-left: 1em;
  border-bottom: 2px solid transparent;
  border-radius: 2px;
  transition: ease-in-out 0.2s;
  white-space: nowrap;
}

.menu li a:hover {
  border-bottom: 2px solid #FBAC00;
  border-radius: 2px;
  color: #2B69DD;
}
.login_container{
  display: flex;
  flex-flow: row;
  align-items: center;
  gap: 24px
}
.login{
  background: #87B645;
  border-radius: 4px;
  height: 32px;
  width: 200px;
  padding: 16px;
  display: flex;
  align-items: center;
  justify-content: center;

}
.burger{

  display: none;
}
@media screen and (max-width: 1024px){
  .menu{
    display: none;
  }
  .login{
    display: none;
  }
  img{
    margin-left: 16px;
  }
  .burger{
    width: 48px;
    height: 48px;
    background: url("../assets/Icons/ic_burger.svg") center no-repeat;
    display: block;
    margin-right: 16px;
  }
  .header{
    margin-top: 24px;
    justify-content: space-between;
  }
}
@media screen and (max-width: 375px){
  .login{
    display: none;
  }
  .burger{
    width: 48px;
    height: 48px;
    background: url("../assets/Icons/ic_burger.svg") center no-repeat;
    display: block;
  }
}
</style>