<template>
  <div>
    <nav class="navbar">
      <div class="navbar__container">
        <a v-on:click="$emit('menuEvent', 'main')" id="navbar__logo">
          <i class="fas fa-futbol"></i> {{ ldt }}
        </a>

        <div class="navbar__toggle" id="mobile-menu">
          <span class="bar"></span>
          <span class="bar"></span>
          <span class="bar"></span>
        </div>

        <ul class="navbar__menu">
          <li class="navbar__item">
            <a class="navbar__links" v-on:click="$emit('menuEvent', 'main')" >{{ inicio }}</a>
          </li>
          <li class="navbar__item">
            <a class="navbar__links" v-on:click="$emit('menuEvent', 'reservas')">{{ reservas }}</a>
          </li>
          <li class="navbar__item">
            <a class="navbar__links" v-on:click="$emit('menuEvent', 'nosotros')">{{ nosotros }}</a>
          </li>
          <li class="navbar__item">
            <a class="navbar__links" v-on:click="$emit('menuEvent', 'postulate')">{{ postulate }}</a>
          </li>
          <li class="navbar__item">
            <a class="navbar__links" v-on:click="$emit('menuEvent', 'sedes')">{{ sedes }}</a>
          </li>
          <li class="navbar__btn">
            <button class="button" ><a href="#" id="ins">{{ sesion }}</a></button>
          </li>
        </ul>

      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  methods: {},
  data (){
    return{
      ldt: "LÍNEA DE TRES",
      inicio: "Inicio",
      reservas: "Reservas",
      nosotros: "Nosotros",
      postulate: "Postulate",
      sedes: "Sedes",
      sesion: "Iniciar Sesión"
    }
  }
}
</script>

<style scoped>
@import "../assets/css/styles.css";
</style>