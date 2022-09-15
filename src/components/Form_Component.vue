<template>
<div class="form_container">
  <span class="H2_48_Bold">Как с нами связаться?</span>
  <span class="Text_Main_18_Regular">Если у вас остались вопросы мы с радостью ответим на них, а так же подробнее расскажем
о нашем продукте.</span>
  <form class="Other_14_regular">
    <input type="text" placeholder="Ваше имя">
    <input type="email" placeholder="E-mail">
    <input type="tel" placeholder="Номер телефона">
    <div class="checkbox_container">
      <input type="checkbox" v-on:click="checkbox">
      <span>Я принимаю условия на <a href="#">обработку персональных данных</a>  <br/>Обещаем, не передавать информацию 3 лицам</span>
    </div>
  </form>
  <span class="Other_18_Medium button "> Отправить</span>
</div>
</template>

<script>
export default {
  name: "Form_Component",
  methods:{
    checkbox (event){
      event.target.parentElement.classList.toggle("active")
    }
}
}
</script>

<style scoped>
.form_container{
  display: flex;
  flex-flow: column;
  align-items: center;
  padding-top: 140px;
  padding-bottom: 127px;
  background: url("../assets/bg/spot5.png") 70% 5% no-repeat;
  background-size: 77%;

  overflow: auto;
}
.Text_Main_18_Regular{
  max-width: 472px;
  text-align: center;
  margin-top: 56px;
}
form{
  display: flex;
  flex-flow: column;
  gap: 16px;
  width: 446px;
  margin-top: 104px;
}

form > input{
  width: 100%;
  padding: 8px 16px;
  height: 38px;
  border: 1px solid #D7D7D7;
  border-radius: 4px;
}
.checkbox_container{
  width: 466px;
  display: flex;
  flex-flow: row;
  gap: 16px;
  margin-top: 16px;
  line-height: 29px;
}
.checkbox_container span{
  color: #F5F5F5;
}
.checkbox_container input{
  width: 24px;
  height: 24px;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;

}
.checkbox_container input:hover::before{
  border: 1px solid #FBAC00;
}
.checkbox_container input::before{
  content: "";
  width: 24px;
  height: 24px;
  background: transparent;
  border: 1px solid #D7D7D7;
  border-radius: 1px;
  display: inline-block;
  position: relative;
  z-index: 0;
}
.checkbox_container.active input::before{
  background: #87B645 url("../assets/Icons/ic_check.png") center no-repeat;
  background-size: 15px;
}

.checkbox_container a {
  color: #FBAC00;
  border-bottom: 2px solid #FBAC00;
  border-radius: 2px;
}

.button {
  width: 232px;
  height: 36px;
  margin-top: 39px;
  padding: 18px;
  background: #87B645;
  border-radius: 4px;
  font-size: 24px;
  line-height: 24px;
  color: white;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}
.button:hover{
  background: #FBAC00;
  color:white;
}
.button:active{
  background: #2B69DD;
  color: #75ACFE;
}
</style>