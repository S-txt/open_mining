<template>
<div class="faq">
  <span class="H2_48_Bold">FAQ</span>
  <div class="faq_container">
    <div class="faq_cards">
      <div class="card"
          v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Что такое майнинг криптовалют?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Что такое хэшрейт?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Сколько я заработаю?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Как начать работать с сервисом?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Как это работает?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Зачем мне регистрироваться <br>на стороннем пуле?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Почему сейчас необходимо <br>использовать пул для майнинга Pool.in</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Почему я не могу получать сразу <br>выплаты с вашего сервиса?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>
      <div class="card"
           v-on:click="toggle">
        <div class="card_title_container">
          <span class="Other_30_Bold card_title">Какие преимущества нашего сервиса <br>облачного майнинга  перед другими?</span>
          <div class="card_arrow"/>
        </div>
        <span class="Text_Main_18_Regular card_content">Криптовалюты добывается оборудованием для майнинга, которое используют свои вычислительные мощности для возможности обработки транзакций и получения вознаграждений. Точнее говоря, майнинг - это процесс записи транзакций в блокчейн и получение
  за это вознаграждения.</span>
      </div>




  </div>
    <div class="faq_help">
      <span class="H3_36_Bold">Остались вопросы<br>и нужна помощь?</span>
      <span class="Text_Main_18_Regular">Напишите нам на <a href="mailto:">почту</a> и мы постараемся решить ваш вопрос</span>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "FAQ_Component",
  methods:{
    toggle (event){
      event.target.classList.toggle("active")
    }
  }
}
</script>

<style scoped>
.faq{
  display: flex;
  align-items: center;
  flex-flow: column;
  width: 100%;
  background: url("../assets/bg/spot4.png") right top no-repeat;
  background-size: 696px 1879px;
  padding-top: 139px;

  overflow: auto;
}
.faq .H2_48_Bold{
  margin-bottom: 69px;
}
.faq_container{
  width: 100%;
  display: flex;
  flex-flow: row;
  justify-content: space-around;
  flex-wrap: nowrap;
}
.faq_cards{
  display: flex;
  flex-flow: column;
  gap:24px;
  max-width: 776px;

}
.card{
  display: flex;
  flex-flow: column;
  cursor: pointer;
  transition: ease-in 0.5s;
  overflow: hidden;
}
.card.active > .card_content{
  max-height: 300px;
  margin-top: 20px;
}
.card_title_container{
  padding: 48px 40px 48px 40px;
  background: #87B645;
  border-radius: 10px;
  transition: ease-in 0.5s;
  display: flex;
  flex-flow: row;
  justify-content: space-between;
  align-items: center;
  pointer-events: none;
  height: 56px;
}
.card_title{
  text-justify: auto;
  z-index: 0;
  color: #F5F5F5;
  transition: ease-in 0.5s;
}
.card_content{
  margin-top: 0;
  max-height: 0;
  transition: ease-in-out 0.5s;
}
.card_arrow{
  content: "";
  width: 30px;
  height: 30px;
  background: url("../assets/Icons/ic_arrow.png") center no-repeat;
  background-size: 32px;
  position: relative;
  z-index: 0;
  float: right;
  transition: ease-in 0.5s;
}
.card.active .card_arrow{
  transform:rotate(90deg) ;
}
.card.active > .card_title_container{
  background:#F8DB73;

}
.card.active > .card_title_container .card_title{
  color: #333333;
}
.faq_help{
  display: flex;
  flex-flow: column;
  width: 472px;
}
.faq_help a {
  color:#2B69DD;
  text-decoration: #FBAC00 underline;
}
</style>