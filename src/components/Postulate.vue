<template>
  <div>
    <div class="main">
      <div class="main__container">
        <div class="main__content">
          <h1>{{titulo}}</h1>
          <p>{{datos}}</p>
        </div>
        <div class="main__img--container">
          <img src="../assets/img/pic5.svg" alt="pic" id="main__img">
        </div>
      </div>
    </div>
    <div class="form-container">
      <div class="form">
        <form action="" class="form-items">
          <h1>¡Postulate acá!</h1>
          <div class="form-validation">
            <label class="control-label">Sede:</label>
            <input type="text" class="form-control" name="fname" id="fname">
          </div>

          <div class="form-validation">
            <label class="control-label">Localidad:</label>
            <input type="text" class="form-control" name="lname" id="lname">
          </div>

          <div class="form-validation">
            <label class="control-label">Dirección:</label>
            <input type="number" class="form-control" name="edad" id="edad">
          </div>

          <div class="form-validation">
            <label class="control-label">Canchas</label>
            <select id="sexo" name="sexo" required="">
              <option selected="" disabled="">Nro Disponible</option>
              <option>1-3</option>
              <option>4-6</option>
              <option>Más de 6</option>
            </select>
          </div>

          <div class="form-validation">
            <label class="control-label">Email:</label>
            <input type="text" class="form-control" name="email" id="email">
          </div>

          <div class="form-validation">
            <label class="control-label">Teléfono:</label>
            <input type="tel" class="form-control" name="tel" id="tel">
            <br>
            <small>EJ: 11-2345-6789</small>
          </div>


          <div class="form-validation">
            <label class="control-label">Preferencia</label>
            <select id="sede" name="sede" required="">
              <option selected="" disabled="">Canchas a postular</option>
              <option>Fútbol 11</option>
              <option>Fútbol 7</option>
              <option>Fútbol 5</option>
            </select>
          </div>

          <div class="form-validation">
            <label class="control-label">Sponsors</label>
            <select id="sede" name="sede" required="">
              <option selected="" disabled="">¿Cuenta con sponsors?</option>
              <option>Si</option>
              <option>No</option>
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
  name: "Postulate",
  data(){
    return {
    titulo:"¡POSTULATE PARA PODER SER SEDE!",
    datos: "Dejanos tus datos para poder formar parte de LDT." ,
    }
  }
}
</script>

<style scoped>
@import "../assets/css/styles.css";
@import "../assets/css/reservas.css";
</style>