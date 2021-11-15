<template>
  <div>
    <div class="main">
      <div class="main__container">
        <div class="main__content">
          <h1>{{ reserva }}</h1>
          <p>{{ registrate }}</p>
        </div>
        <div class="main__img--container">
          <img src="../assets/img/App.svg" alt="pic" id="main__img">
        </div>
      </div>
    </div>

    <div class="form-container">
      <div class="form">
        <form action="" class="form-items">
          <h1>Hacé tu Reserva</h1>
          <div class="form-validation">
            <label class="control-label">Nombre:</label>
            <input type="text" class="form-control" name="fname" id="fname">
          </div>

          <div class="form-validation">
            <label class="control-label">Apellido:</label>
            <input type="text" class="form-control" name="lname" id="lname">
          </div>

          <div class="form-validation">
            <label class="control-label">Edad:</label>
            <input type="number" class="form-control" name="edad" id="edad">
          </div>

          <div class="form-validation">
            <label class="control-label">Sexo:</label>
            <select id="sexo" name="sexo" required="">
              <option selected="" disabled="">Elegir sexo</option>
              <option>Femenino</option>
              <option>Masculino</option>
              <option>Otro</option>
            </select>
          </div>

          <div class="form-validation">
            <label class="control-label">Email:</label>
            <input type="text" class="form-control" name="email" id="email">
          </div>

          <div class="form-validation">
            <label class="control-label">Teléfono:</label>
            <input type="tel" class="form-control" name="tel" id="tel">
          </div>


          <div class="form-validation">
            <label class="control-label">{{ sede }}</label>
            <select id="sede" name="sede" required="">
              <option selected="" disabled="">{{ sede }}</option>
              <option>Escobar</option>
              <option>Lanús</option>
              <option>Moreno</option>
              <option>Palermo</option>
            </select>
          </div>

          <div class="form-validation">
            <label class="control-label">Fecha y Hora</label>
            <input type='datetime-local' class="form-control" />
          </div>

          <div class="form-validation">
            <label class="control-label">{{ categoria }}</label>
            <select id="sede" name="sede" required="">
              <option selected="" disabled="">{{ categoria }}</option>
              <option>Fútbol 11</option>
              <option>Fútbol 7</option>
              <option>Fútbol 5</option>
            </select>
          </div>


          <input type="submit" class="btn btn-primary" value="Submit">
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Reservas",
  data(){
    return{
      reserva:"¡REALIZÁ TU RESERVA ACÁ!",
      registrate: "Registrate más abajo para poder jugar",
      categoria:"Elegir Categoría",
      sede:"Elegir Sede",
    }
  }
}
</script>

<style scoped>
@import "../assets/css/styles.css";
@import "../assets/css/reservas.css";

</style>