<template>
  <div>
    <div class="form-container">
      <div class="form">
      <form class="form-items" id="login">
        <h1>Iniciar Sesión</h1>

        <div class="form__input-group">
          <input type="text" class="form__input" autofocus placeholder="Username or email">
          <div class="form__input-error-message"></div>
        </div>
        <div class="form__input-group">
          <input type="password" class="form__input" autofocus placeholder="Password">
          <div class="form__input-error-message"></div>
        </div>
        <button class="form__button" type="submit">Continuar</button>
        <p class="form__text">
          <a href="#" class="form__link">¿Olvidaste tu contraseña?</a>
        </p>
        <p class="form__text">
          <a class="form__link" href="./" id="linkCreateAccount">¿No tenes una cuenta? Create una acá</a>
        </p>
      </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Login"
}
</script>

<style scoped>
@import "../assets/css/styles.css";
@import "../assets/css/login.css";
@import "../assets/css/reservas.css";
</style>