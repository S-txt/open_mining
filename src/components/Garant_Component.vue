<template>
<div class="garant_container">
  <span class="H2_48_Bold">Гарантии</span>
  <div class="garant_cards">
    <div class="card" id="card_1">
      <span class="H4_24_Bold">Наша компания зарегистрирована<br> не в офшорных зонах</span>
      <span class="Text_Main_18_Regular">Мы являемся резидентами Российской Федерации, у нас есть собственная площадка для размещения оборудования в Иркутской области. </span>
    </div>
    <div class="card" id="card_2">
      <span class="H4_24_Bold">Подтверждено публичным пулом pool.in</span>
      <span class="Text_Main_18_Regular">Мы продаем контракты на облачный майнинг из уже имеющегося оборудования</span>
      <a href="#card_2"></a>
    </div>
    <div class="card" id="card_3">
      <span class="H4_24_Bold">Никаких скрытых <br>действий</span>
      <span class="Text_Main_18_Regular">Вся финансовая отчетность о нашей компании опубликована в свободном доступе. Вы можете её найти по ИНН.</span>
      <a href="#card_3"></a>
    </div>
  </div>
  <div class="graph">
    <img src="../assets/img/Graph.png">
    <span class="Text_Main_18_Regular">Наши возможности:  <a href="">https://www.poolin.com/my/9053220/b...</a></span>

  </div>
</div>
</template>

<script>
export default {
  name: "Garant_Component"
}
</script>

<style scoped>
.garant_container{
  padding-top: 227px;
  display: flex;
  align-items: center;
  flex-flow: column;
  width: 100%;
  gap: 72px;
  background: url("../assets/bg/spot3.png") 63% 5% no-repeat;
  background-size: 40%;

  overflow: auto;
}
.garant_cards{
  display: flex;
  flex-flow: row;
  gap: 52px;
  flex-wrap: wrap;
}
.card{
  display: flex;
  flex-flow: column;
  width: 400px;
  height: 296px;
  box-shadow: 0 4px 20px rgba(165, 165, 165, 0.25);
  border-radius: 8px;
  padding: 32px;
  gap: 16px;
}

.card a{
  position: relative;
  width: 48px;
  height: 48px;
  background: #87B645
  url("../assets/Icons/ic_arrow.png") center no-repeat;
  background-size: 21px;
  border-radius: 8px;
  top: 75px;
  transition: 0.3s ease;
}
.card a:hover{
  background: #FBAC00
  url("../assets/Icons/ic_arrow.png") center no-repeat;
  background-size: 21px;

}
.card a:active{
  background: #2B69DD
  url("../assets/Icons/ic_arrow_active.png") center no-repeat;
  background-size: 21px;
  color: #75ACFE;

}

#card_1{
  background: #F8DB73
  url("../assets/bg/01.png") right 2% no-repeat;
  background-size: 160px 112px;
}
#card_2{
  background: #A0C4FA
  url("../assets/bg/02.png") right 2% no-repeat;
  background-size: 192px 112px;
}
#card_3{
  background: #FFFFFF
  url("../assets/bg/03.png") right 2% no-repeat;
  background-size: 192px 112px;
}
.graph{
  display: flex;
  flex-flow: column;
  align-items: center;
  gap:55px
}
img{
  width: 40%;
  padding: 10px;
  border-radius: 8px;
  background: #FFFFFF;
  box-shadow: 0 4px 20px rgba(165, 165, 165, 0.25);
}
.graph span{
  background: url("../assets/Icons/ic_atention.png") left no-repeat;
  background-size: 32px;
  padding-left: 48px ;
}
.graph a{
  color: #75ACFE;
  text-decoration: underline;
}
</style>