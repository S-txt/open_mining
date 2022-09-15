<template>
  <div class="tab">
    <div class="card">
      <img src="../../src/assets/Icons/ic_risk.png">
      <span class="H4_24_Bold">Все риски берем на себя</span>
      <span class="Text_Main_18_Regular">Покупка оборудование, его транспортировка, размещение, оплата электричества, ремонт и сопровождение — все эти риски мы берем на себя</span>
    </div>
    <div class="card">
      <img src="../../src/assets/Icons/ic_honest.png">
      <span class="H4_24_Bold">Гарантия честности схемы работы</span>
      <span class="Text_Main_18_Regular">Вы покупаете только мощность оборудования — хешрайт, так заключается контракт. Купленная мощность направляется на один из пулов, который вы выбираете. Сторонний пул гарантирует прозрачность, честность и простоту схемы</span>
    </div>
    <div class="card">
      <img src="../../src/assets/Icons/ic_clearpay.png">
      <span class="H4_24_Bold">Никаких скрытых платежей</span>
      <span class="Text_Main_18_Regular">Никаких ежедневных списаний за обслуживание и электроэнергию. Короткие контракты на 3 месяца, минимизируют риски, что майнинг станет невыгоден вследствие роста сложности, халвинга и падение курсов</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Tab_Component"
}
</script>

<style scoped>
.tab{
  align-items: center;
  display: flex;
  text-align: center;
  width: 100%;
  column-gap: 80px;
  justify-content: center;
  margin: 110px 0 0;
}
.tab .card{
  width: 416px;
  height: 552px;
  border: 1px solid #D7D7D7;
  border-radius: 24px;
  display: flex;
  flex-flow: column;
  align-items: center;
  -webkit-transition: 1s ease; /* Safari and Chrome */
  -moz-transition: 1s ease; /* Firefox 4 */
  -o-transition: 1s ease; /* Opera */
}
.tab .card img{
  width: 176px;
  height: 176px;
  margin: 32px 0 16px 0
}
.tab .card span{
  margin: 10px 24px;
}
.tab .card:hover{
  transform: translateY(-10px);
}

</style>