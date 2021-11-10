<template>
  <div>
    <div class="main">
      <div class="main__container">
        <div class="main__content">
          <h1>NUEVA MANERA</h1>
          <h2>DE VIVIR EL FÚTBOL</h2>
          <p>Conocé nuestro servicio</p>
          <button class="main__btn" id="main__btn"><a href="#">Inscribírse</a></button>
        </div>
        <div class="main__img--container">
          <img src="../assets/img/pic5.svg" alt="pic" id="main__img">
        </div>
      </div>
    </div>

    <div class="services">
      <h1>{{ enterate }}</h1>
      <div class="services__container">
        <div class="services__card">
          <h2>Hacé tu Reserva</h2>
          <p>Fechas y Horarios</p>
          <button>
            <a class="comenzar" v-on:click="$emit('menuEvent','reservas')"> Comenzar </a>
          </button>
        </div>
        <div class="services__card">
          <h2>Postulate</h2>
          <p>Unite a la comunidad</p>
          <button>
            <a class="comenzar" v-on:click="$emit('menuEvent','postulate')"> Comenzar </a>
          </button>
        </div>
      </div>
    </div>
  </div>


</template>

<script>
export default {
  name: "Main",
  data(){
    return{
      enterate:"Enterate de Nuestros Servicios",

    }
  }
}
</script>

<style scoped>
@import "../assets/css/styles.css";
</style>