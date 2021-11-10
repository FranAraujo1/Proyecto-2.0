<template>
  <div>

    <div class="footer__container">
      <div class="footer__links">
        <div class="footer__link--wrapper">
          <div class="footer__link--items">
            <h2>{{ nosotros }}</h2>
            <a>{{ que_hacemos }}</a>
            <a>{{ servicios }}</a>
            <a>{{ sede }}</a>
            <a>{{ sponsors }}</a>
          </div>
          <div class="footer__link--items">
            <h2>Contacto</h2>
            <a>{{ contacto }}</a>
            <a>{{ soporte }}</a>
            <a>{{ opinion }}</a>
          </div>
        </div>
        <div class="footer__link--wrapper">
          <div class="footer__link--items">
            <h2>{{ terminos }}</h2>
            <a>{{ terminos }}</a>
            <a>{{ politica }}</a>
            <a>{{ Influencers }}</a>
          </div>
          <div class="footer__link--items">
            <h2>{{ redes }}</h2>
            <a>{{ insta }}</a>
            <a>{{ face }}</a>
            <a>{{ you }}</a>
            <a>{{ twitter }}</a>
            <a>{{ tik }}</a>
          </div>
        </div>
      </div>

      <div class="social__media">
        <div class="social__media--wrap">
          <div class="footer__logo">
            <a href="/" id="footer__logo"><i class="fas fa-futbol"></i>{{ ldt }}</a>
          </div>
          <p class="website__rights">{{ derechos }}</p>
          <div class="social__icons">
            <a href="http://facebook.com/" class="social__icon--link" target="_blank">
              <i class="fab fa-facebook"></i>
            </a>
            <a href="/" class="social__icon--link" target="_blank">
              <i class="fab fa-instagram"></i>
            </a>
            <a href="/" class="social__icon--link" target="_blank">
              <i class="fab fa-twitter"></i>
            </a>
            <a href="/" class="social__icon--link" target="_blank">
              <i class="fab fa-linkedin"></i>
            </a>
            <a href="/" class="social__icon--link" target="_blank">
              <i class="fab fa-youtube"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data(){
    return {
      nosotros:"Nosotros",

      que_hacemos: "Qué Hacemos",
      servicios: "Otros Servicios",
      sede: "Sede Oficial",
      sponsors:"Sponsors",

      contacto:"Contacto",
      soporte:"Soporte",
      opinion:"Opinión",

      terminos:"Términos y Condiciones",
      politica:"Política de Privacidad",
      influencers:"Influencers",

      redes:"Redes",
      insta:"Instagram",
      face:"Facebook",
      you:"Youtube",
      twitter:"Twitter",
      tik:"TikTok,",

      ldt:"LÍNEA DE TRES",
      derechos:"LDT 2021. Todos los derechos reservados"


    }
  }
}
</script>

<style scoped>
@import "../assets/css/styles.css";

</style>