<template>
  <div class="container">
    <Header_Component/>
    <Main_Component/>
    <About_Component/>
<!--    <Tab_Component/>-->
    <Edge_Component/>
    <Calc_Component/>
    <Garant_Component/>
    <FAQ_Component/>
    <Form_Component/>
    <Footer_Component/>
  </div>
</template>

<script>
import Header_Component from "@/components/Header_Component";
import Main_Component from "@/components/Main_Component";
import About_Component from "@/components/About_Component";
// import Tab_Component from "@/components/Tab_Component";
import Edge_Component from "@/components/Edge_Component";
import Calc_Component from "@/components/Calc_Component";
import Garant_Component from "@/components/Garant_Component";
import FAQ_Component from "@/components/FAQ_Component";
import Form_Component from "@/components/Form_Component";
import Footer_Component from "@/components/Footer_Component";
export default {
  name: 'App',
  components: {
    Footer_Component,
    Form_Component,
    FAQ_Component,
    Garant_Component,
    Calc_Component,
    Edge_Component,
    // Tab_Component,
    About_Component,
    Main_Component,
    Header_Component
  },
  data(){
    return{

      dropdown_value:"BTC",
      dropdown_img: "../assets/Icons/Drop/" + this.dropdown_value +".png"
    }
  }
}
</script>

<style>
@import "assets/Fonts.css";
html{
  font-size: 16px;
  overflow: auto;
}

body{
  margin: 0;
  background: #F5F5F5;
  /*min-width: 1768px;*/
}
*{
  font-family: 'Gotham Pro', sans-serif;
  text-decoration: none;
  color: black;
  /*box-sizing: border-box;*/
}
li{
  list-style: none;
}
@media screen and (max-width: 375px){
  html{
    font-size: 9px;
    overflow: auto;
  }
}
</style>
