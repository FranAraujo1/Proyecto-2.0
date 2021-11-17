<template>
  <div class="modal" id="email-modal">
    <div class="modal-content">

      <div class="modal-content-left">
        <img src="../assets/img/pic1.svg" alt="" id='modal-img'>
      </div>
      <div class="modal-content-right">
        <form  method="GET" class="modal-form" id="form">
          <h1>{{unite}}</h1>
          <div class="form-validation">
            <input type="text" required v-model="name" class="modal-input" id="name" name="name" placeholder="Ingresá tu nombre">
            <p>Error Message</p>
          </div>
          <div class="form-validation">
            <input type="email" class="modal-input" id="email" name="email" placeholder="Ingresá tu mail">
            <p>Error Message</p>
          </div>
          <div class="form-validation">
            <input type="password" class="modal-input" id="password" name="password"
                   placeholder="Ingresá tu contraseña">
            <p>Error Message</p>
          </div>
          <div class="form-validation">
            <input type="password" class="modal-input" id="password-confirm" name="password"
                   placeholder="Confirmá tu contraseña">
            <p>Error Message</p>
          </div>
          <input type="submit" class="modal-input-btn" value="Sign Up">
          <div class="modal-input-login">¿Ya tenes una cuenta? Iniciá sesión
            <a v-on:click="$emit('menuEvent','login')">acá</a>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "inscribite",
  methods: {
/*    altaNombre() {
       axios.post("http://localhost:5000/api/v1/nombre"),
           {
             name: this.name,
           }
    }*/
  },
  data () {
    return {
     unite: "¡Unite a nosotros hoy! Crea tu cuenta completando la información de abajo.",
    }
  }
}

</script>

<style scoped>
@import "../assets/css/styles.css";
@import "../assets/css/modal.css";
</style>