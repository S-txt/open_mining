<template>
  <div class="calc_container">
    <span class="H2_48_Bold">Расчитайте свой доход</span>
    <div class="calc">
      <div class="calc_item">
        <span class="Text_Main_18_Regular">Мощность,  Th/ s</span>
        <input type="number"
               min="10"
               max="1000"
               id="power_input"
               class="Other_18_Medium"
               v-model="power_value"
        >
        <input type="range"
               min="10"
               max="1000"
               v-model="power_value"
               id="power_range">
        <div class="calc_footer Other_14_regular">
          <span>10 Th/ s</span>
          <span>1000 Th/ s</span>
        </div>
      </div>
      <div class="calc_item">
        <span class="Text_Main_18_Regular">Срок контракта, дни</span>
        <input type="number"
               min="90"
               max="365"
               id="term_input"
               class="Other_18_Medium"
               v-model="term_value">
        <input type="range"
               min="90"
               max="365"
               v-model="term_value"
               id="term_range">
        <div class="calc_footer Other_14_regular">
          <span>90 дней</span>
          <span>365 дней</span>
        </div>
      </div>
      <div class="calc_item">
        <span class="Text_Main_18_Regular">Вид валюты</span>
        <div class="calc_dropdown Other_18_Medium">
          <input type="text"
                 class="Other_18_Medium"
                 placeholder="{{dropdown_value}}"
                 id="{{dropdown_value}}"
                 v-model="dropdown_value"
                 v-on:click.prevent="!dropdown_visible"
                 style='visibility:"{{dropdown_visible}}"'>
          <div class="calc_dropdown_option" >
            <div id="BTC">BTC</div>
            <div id="LTC">LTC</div>
            <div id="RPL">RPL</div>
            <div id="ETH">ETH</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Calc_Component",
  data(){
    return{
      power_value:10,
      term_value:90,
      dropdown_value: "BTC",
      dropdown_visible: "hidden",
      dropdown_open: false
    }
  }
}
</script>

<style scoped>
.calc_container{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-flow: column;
  width: 100vw;

  overflow: auto;
}
.calc{
  display: flex;
  gap: 65px;
  margin-top: 70px;
  flex-wrap: wrap;
}
.calc_item{
  display: flex;
  flex-flow: column;
  width: 426px;

}
.calc_footer{
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.calc_footer span{
  color: #A1A1A3;
}
.calc_item input{
  margin: 8px 0
}
.calc_item input[type = number]{

  padding: 20px 24px;
  border: 1px solid #D7D7D7;
  border-radius: 8px;
  background: #FFFFFF;
}

.calc_item input[type = number]:focus{
  outline: none;

}

input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  /* display: none; <- Crashes Chrome on hover */
  -webkit-appearance: none;
  margin: 0; /* <-- Apparently some margin are still there even though it's hidden */
}

.calc_item input[type = range]{
  -webkit-appearance: none;
  width:100%;
  height: 2px;
  outline: none;
  border-radius: 3px;
  background: #FBAC00;
  accent-color: #F55050;
}
::placeholder { /* Chrome, Firefox, Opera, Safari 10.1+ */
  color: black;
  opacity: 1; /* Firefox */
}

:-ms-input-placeholder { /* Internet Explorer 10-11 */
  color: black;
}

::-ms-input-placeholder { /* Microsoft Edge */
  color: black;
}
.calc_item .calc_dropdown input[type = text] {
  padding: 20px 24px;
  border: 1px solid #D7D7D7;
  border-radius: 8px;
  background: #FFFFFF;
  margin: 8px 0;
  cursor: pointer;
  color: black;
  width: 376px;
}
.calc_item .calc_dropdown_option {
  position: relative;
  padding: 20px 24px;
  border: 1px solid #D7D7D7;
  border-radius: 8px;
  background: #FFFFFF;
}
.calc_item .calc_dropdown_option div{
  padding: 20px 47px;
  margin: 8px 0;
  background: left no-repeat;
  background-size: 32px;
}
.calc_dropdown .calc_dropdown_option div:hover{
  background: #FBAC00;
  cursor: pointer;
  border-radius: 8px;
}





.calc_item input[type = range]::-moz-range-progress{
  accent-color: #F55050;
}
.calc_item input[type = range]::-webkit-slider-thumb{
  -webkit-appearance: none;
  width: 22px;
  height: 22px;
  position: relative;
  background: #87B645;
  border: 1px solid #FBAC00;
  border-radius: 50%;
  cursor: pointer;
}
#BTC{
  background-image: url("../assets/Icons/Drop/BTC.png");
  background-position: 2% 50%;
  background-repeat: no-repeat;
  background-size: 32px;

}
#LTC{
  background-image: url("../assets/Icons/Drop/LTC.png");
  background-position: 2% 50%;
  background-repeat: no-repeat;
  background-size: 32px;
}
#RPL{
  background-image: url("../assets/Icons/Drop/RPL.png");
  background-position: 2% 50%;
  background-repeat: no-repeat;
  background-size: 32px;
}
#ETH{
  background-image: url("../assets/Icons/Drop/ETH.png");
  background-position: 2% 50%;
  background-repeat: no-repeat;
  background-size: 32px;
}
</style>