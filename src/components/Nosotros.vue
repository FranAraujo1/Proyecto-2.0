<template>
  <div>
    <div class="main">
      <div class="main__container">
        <div class="main__content">
          <h1>SOMOS LÍNEA DE TRES</h1>
          <p>¡CONOCÉNOS!</p>
        </div>
        <div class="main__img--container">
          <img src="../assets/img/nosotros2.svg" alt="pic" id="main__img">
        </div>
      </div>
    </div>

    <main class="sedes">
      <h1>¡CONOCÉ MÁS SOBRE NOSOTROS!</h1>
      <div class="sedes_container">
        <section class="card__sede">
          <div class="titulo__card--sede">
            <h3 class="titulo__sede">¿QUÉ HACÉMOS?</h3>
          </div>
          <figure>
            <img class="imagen__sede" src="../assets/img/lineup.png" alt="Sede Zona Norte">
          </figure>
          <figcaption>
            <div class="box_tres">
              <p>{{conectamos}}</p>
            </div>
          </figcaption>
        </section>
        <section class="card__sede">
          <h3 class="titulo__sede">¿CÓMO LO HACEMOS?</h3>
          <figure>
            <img class="imagen__sede" src="../assets/img/conectamos.png" alt="Sede Zona Sur">
          </figure>
          <figcaption>
            <div class="box_tres">
              <p>{{ usuarios }}</p>
            </div>
          </figcaption>
        </section>
        <section class="card__sede">
          <h3 class="titulo__sede">SIEMPRE DAMOS EL EXTRA</h3>
          <figure>
            <img class="imagen__sede" src="../assets/img/conos.png" alt="Sede Zona Oeste">
          </figure>
          <figcaption>
            <div class="box_tres">
              <p>
                {{brindamos}}
              </p>
            </div>
          </figcaption>
        </section>
        <section class="card__sede">
          <h3 class="titulo__sede">SPONSORS</h3>
          <figure>
            <img src="../assets/img/gatorade.png" alt="Sede Capital Federal" class="imagen__sede">
          </figure>
          <figcaption>
            <div class="box_tres">
              <P>
                {{contamos}}
              </P>
            </div>
          </figcaption>
        </section>
      </div>
    </main>

  </div>
</template>

<script>
export default {
  name: "Nosotros",
  methods: {},
  data () {
    return {
      conectamos: "Conenctamos clubes con jugadores para que vivan una experiencia única.Transmitimos la pasión de vivir el fútbol ahora en la web, llevando el deporte más famoso del mundo a la plataforma más usada en el mundo.La experiencia de usuario conecta lo digital con lo físico.",
      usuarios:"Los usuarios se dan de alta en la aplicación y se postulan para ser nuevas sedes de Línea de Tres. Simultaneamente, aquellos que quieren jugar con amigos al fútbol y no encuentran la manera, también se inscriben para reservar su espacio.",
      brindamos:"Brindamos servicios de pecheras por si no se distinguen las camisetas. Proveemos bares y confiterías en varias de nuestras sedes. Equipamos las sedes con conos, pelotas, banderines, planillas, infladores y todo aquello que se necesita para llevar acabo el juego y el post juego",
      contamos:"Contamos con más de 10 sponsors.Entre ellos se encuentran: Gatorade, Quilmes, Penalty, Umbro, Kappa, Vairo, Motomel, Volskwagen, Mercado Libre y Hells Pizza.Ellos nos brindan el apoyo necesario para llevar adelante el negocio."
    }
  }
}
</script>

<style scoped>
@import "../assets/css/styles.css";
@import "../assets/css/sedes.css";
</style>