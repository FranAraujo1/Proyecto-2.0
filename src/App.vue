<template>
  <div id="app">

    <NavBar v-on:menuEvent="showMenuOption($event)"/>

    <div id="main-container">
      <div>
        <Main v-if="menu.main" v-on:menuEvent="showMenuOption($event)"/>
        <Reservas v-if="menu.reservas"/>
        <Nosotros v-if="menu.nosotros"/>
        <Postulate v-if="menu.postulate"/>
        <Sedes v-if="menu.sedes"/>
        <Login v-if="menu.login"/>
        <inscribite v-if="menu.inscribite"/>
      </div>



      <Banner/>





    </div>

    <Footer/>
  </div>
</template>

<script>

import Main from './components/Main';
import NavBar from "./components/NavBar";
import Reservas from "./components/Reservas";
import Nosotros from "./components/Nosotros";
import Sedes from "./components/Sedes";
import Banner from "./components/Banner";
import Footer from "./components/Footer";
import Postulate from "./components/Postulate";
import Login from "./components/Login";
import inscribite from "./components/inscribite";




export default {
  name: 'App',
  components: {
    Footer,
    Sedes,
    Nosotros,
    Reservas,
    NavBar,
    Main,
    Banner,
    Postulate,
    Login,
    inscribite,
  },
  data(){
    return {
      menu:{
        activeOption:"main",
        main:true,
        reservas:false,
        nosotros:false,
        postulate:false,
        sedes: false,
        login: false,
        inscribite: false,
      }
    }
  },
  methods: {
    showMenuOption(option){
      let oldOption = this.menu.activeOption;
      this.menu.activeOption = option;

      this.menu[oldOption] = false;
      this.menu[this.menu.activeOption] = true;

    }
  }
}
</script>

<style>
@import "./assets/css/styles.css";
</style>
