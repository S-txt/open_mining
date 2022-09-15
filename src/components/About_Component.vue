<template>
  <div class="about_container">
    <img src="../../src/assets/img/Laptop.png" alt="laptop">
    <div class="about">
      <span class="H2_48_Bold">open mining</span>
      <span class="Text_1_30_Regular">— это прозрачный заработок на майнинге криптовалют, а самое главное — мы находимся в России.</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "About_Component"
}
</script>

<style scoped>
.about_container{
  height: 1300px;
  background:  url("../../src/assets/bg/spot1.png") right no-repeat;
  overflow: hidden;
}
img{

}

.about{
  position: relative;
  top: 20vw;
  left: 65vw;

  display: flex;
  flex-flow: column;

  max-width: 560px;
  height: 213px;

  row-gap: 37px;
  text-align: left;

}
.about .H2_48_Bold{
  color: #1BAAD1;
}
</style>