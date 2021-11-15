<template>
  <div class="modal" id="email-modal">
    <div class="modal-content">
      <span class="close-btn">&times;</span>
      <div class="modal-content-left">
        <img src="./img/pic1.svg" alt="" id='modal-img'>
      </div>
      <div class="modal-content-right">
        <form action="javascript:Validate(id)" method="GET" class="modal-form" id="form">
          <h1>{{unite}}</h1>
          <div class="form-validation">
            <input type="text" class="modal-input" id="name" name="name" placeholder="Ingresá tu nombre">
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
          <span class="modal-input-login">¿Ya tenes una cuenta? Iniciá sesión <a href="#">acá</a></span>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "inscribite"
  methods: {},
  data () {
    return {
     unite: "¡Unite a nosotros hoy! Crea tu cuenta completando la información de abajo.",
    }
  }
}
</script>

<style scoped>
@import "../assets/css/modal.css";
</style>