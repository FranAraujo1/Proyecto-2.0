<template>
  <div>
    <!-- Main Section -->
    <main class="sedes">
      <br>
      <br>
      <h1>{{title}}</h1>
      <div class="sedes_container">
        <section class="card__sede">
          <div class="titulo__card--sede">
            <h3 class="titulo__sede">¿QUÉ HACÉMOS?</h3>
          </div>
          <figure>
            <img class="imagen__sede" src="../assets/img/canchasZonaNorte.png" alt="Sede Zona Norte">
          </figure>
          <figcaption>
            <div class="box_cuatro">
              <p>En zona Norte contamos con 4 canchas de 11 jugadores, en las cuales se pueden dividir en 3 canchas de fútbol
                5 y 7.
                El complejo deportivo Línea de Tres, te provee la indumentaria necesaria para jugar los partidos (pecheras y
                guantes de arquero).
                Posee un quincho con asador, vestuarios y un salon de eventos.
                Para utilizar el quincho y el salon de eventos, deben avisar con una anticipación de 15 días antes de la
                fecha estipulada. Todos los cargos serán abonados en el momento.</p>
            </div>
          </figcaption>
        </section>
        <section class="card__sede">
          <h3 class="titulo__sede">¿CÓMO LO HACEMOS?</h3>
          <figure>
            <img class="imagen__sede" src="../assets/img/canchasZonaSur.png" alt="Sede Zona Sur">
          </figure>
          <figcaption>
            <div class="box_cuatro">
              <p>En zona Sur actualmente contamos con dos canchas de fútbol 11 y están en construccion unas tres
                canchas de futbol 5 y 7.
                Contamos con vestuarios, en los cuales hay duchas y casilleros individuales.
                También por motivos sanitarios y debido a las exigencias del COE, no se entregan vestimentas y los
                vestuarios no pueden utilizarse hasta nuevo aviso.
                Línea de Tres en esta sede tambien cuenta con un kiosco y restaurante para antes o después de los partidos.</p>
            </div>
          </figcaption>
        </section>
        <section class="card__sede">
          <h3 class="titulo__sede">SIEMPRE DAMOS EL EXTRA</h3>
          <figure>
            <img class="imagen__sede" src="../assets/img/canchasZonaOeste.png" alt="Sede Zona Oeste">
          </figure>
          <figcaption>
            <div class="box_cuatro">
              <p>
                En zona Oeste contamos con 3 canchas de fútbol 5 y 7, es la única sede del complejo Línea de 3 que no tiene
                cancha de fútbol 11, por una cuestion de espacio.
                En este caso, contamos con servicio vigente de pecheras y guantes, ya que fuimos autorizados por
                la municipalidad.
                Contamos con vestuarios, salón de eventos, kiosco y bar.
              </p>
            </div>
          </figcaption>
        </section>
        <section class="card__sede">
          <h3 class="titulo__sede">SPONSORS</h3>
          <figure>
            <img src="../assets/img/canchasZonaCapitalFederal.png" alt="Sede Capital Federal" class="imagen__sede">
          </figure>
          <figcaption>
            <div class="box_cuatro">
              <P>
                En la sede de Capital Federal, contamos con una cancha de fútbol 11, la cual se puede dividir en tres
                canchas de fútbol 7 y adicionalmente contamos con dos canchas de fútbol 5.
                Tiene un vestuario el cual está en fase de construcción y con servicio de cantina incluído con el turno.
                En ésta sede contamos con un bar de primer nivel para descansar post-partido.
                Está en proyecto la idea de agregar un salón de eventos y una pileta para la temporada de verano.
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
  name: "Sedes",
  data(){
    return{
      title:"NUESTRAS SEDES",
      sede_uno: "Sede Zona Norte - (Escobar)",
      sede_dos:"Sede Zona Sur - (Lanús)",
      sede_tres:"Sede Zona Oeste - (Moreno)",
      sede_cuatro: "Sede Capital Federal - (Palermo)",
    }
  }
}
</script>

<style scoped>
@import "../assets/css/styles.css";
@import "../assets/css/sedes.css";
</style>