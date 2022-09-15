<template>
    <div class="main_container">
    <span class="H1_60_Bold">
      Снижение рисков связанных с майнингом<br>по максимуму
    </span>
      <span class="Text_2_24_Regular">
      Честность майнинга заложена в архитектуре
    </span>

      <div class="btns">
        <a href="#" class="btn Other_18_Medium" id="btn_1">Начать зарабатывать</a>
        <a href="#" class="btn Other_18_Medium" id="btn_2">Узнать больше</a>
      </div>
    </div>
</template>

<script>
export default {
  name: "Main_Component"
}
</script>

<style scoped>
.main_container{
  display: flex;
  align-items: center;
  flex-flow: column;
  background:
      url("../../src/assets/bg/graph_1.svg") top no-repeat,
      url("../../src/assets/bg/graph_2.svg") left bottom no-repeat;
  background-size: cover;
  padding-top: 140px;
  flex-flow: column;
  justify-content: center;
  width: 100vw;
  row-gap: 56px;
  text-align: center;
}

.main_container ul{
  display: flex;
  justify-content: center;
  margin-top: 3px;
}
.btns{
  display: flex;
  gap: 54px;
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
@media screen and (max-width: 375px){
  .main{
    padding-top: 56px;
  }
  .main_container{
    width: 100%;
    row-gap: 40px;
  }

  #btn_2{
    display: none;
  }
}
</style>