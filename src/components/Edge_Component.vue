<template>
  <div class="edge_container">
    <span class="H2_48_Bold">Преимущества облачного майнинга</span>
    <div class="edge">
      <ul>
        <li class="card_big_alert alert H3_36_Bold">
          Обычный майнинг
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Ожидаете поставки майнеров и теряете драгоценное время.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Тратите время на подготовку оборудования к работе.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Отсутствие достаточного охлаждения снижает эффективность оборудования. Велик риск перегревания и поломки.
          Результат – дополнительные затраты и потеря времени.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Высокая стоимость электроэнергии.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Необходимость уделять много времени обслуживанию оборудование. Результат поломок – потеря времени
          и упущенная прибыль.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Шум от оборудования и избыточное тепло.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Дополнительные расходы на обеспечение безопасности майнеров.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Возможны дополнительные траты на оплату таможенных пошлин при поставке оборудования.
        </li>
        <li class="card_small alert Text_Main_18_Regular">
          Необходимость в специальных знаниях для настройки и поддержания работоспособности майнеров.
        </li>

        <li class="card_big_accept accept H3_36_Bold">
          Облачный майнинг
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Оборудование всегда готово к работе. Просто выбирайте контракт и начинайте зарабатывать.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Просто и удобно. Не нужно ничего настраивать и иметь IT-навыки.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Оптимальные промышленные условия обеспечивают максимальную производительность майнеров.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Низкая стоимость электроэнергии, значит отличные цены
          на всех контрактах.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Бесперебойная работа. 24/7/365 контроль за работой  майнеров. Высочайшие стандарты безопасности.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Тишина и спокойствие.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Гарантия безопасности майнеров.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Отсутствие непредвиденных расходов. Вы платите только один раз и только ту сумму, которая указана в контракте.
        </li>
        <li class="card_small accept Text_Main_18_Regular">
          Квалифицированные специалисты.
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Edge_Component"
}
</script>

<style scoped>
.edge_container{
  display: flex;
  justify-content: center;
  flex-flow: column;
  align-items: center;
  background: url("../assets/bg/spot2.png") 0 15% no-repeat;
  width: 100vw;
  overflow-x: auto;
}
.edge_container .H2_48_Bold{
  margin: 72px 0;
}
.edge{
  display: flex;
  justify-content: center;
  overflow-x: scroll;

}
.card_small{
  display: flex;
  justify-self: center;
  align-items: center;

}
.edge ul{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(10, auto);
  grid-auto-flow: column;
  gap: 24px;
  align-items: stretch;
  justify-content: center;

}
.edge .H3_36_Bold{
  box-sizing: border-box;
  position: relative;
  width: 668px;
  height: 208px;

  border-radius: 12px;
  border-top: 16px solid var(--clr);
  text-align: center;
  padding: 70px 0 0 145px ;
  border-left: none;
}
.alert{
  --clr:#EB5757
}
.accept{
  --clr:#87B645
}
.edge .card_big_alert{
  background:
      url("../../src/assets/bg/edge_alert.png") right no-repeat,
      url("../../src/assets/Icons/ic_allert.png") 10% no-repeat,
      #E7E9E8;
  background-size:20%;
}
.edge .card_big_accept{
  background:
      url("../../src/assets/bg/edge_accept.png") right no-repeat,
      url("../../src/assets/Icons/ic_accept.png") 10% no-repeat,
      #E7E9E8;
  background-size:20%;
}
.edge .card_small{
  width: 584px;
  padding: 24px 16px 24px 32px;
  border-left: 8px solid var(--clr);
  border-radius: 8px;
}
.edge .card_small:nth-child(2n){
  background: #E7E9E8;
}

@media screen and (max-width: 768px){
  .edge{
    overflow-x: scroll;

  }

}


</style>