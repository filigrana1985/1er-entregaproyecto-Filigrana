<template>
    <div>
      <h2>Iniciar sesión</h2>
      <form @submit.prevent="login">
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email" v-model="email" class="form-control" required>
        </div>
        <div class="form-group">
          <label for="password">Contraseña:</label>
          <input type="password" id="password" v-model="password" class="form-control" required>
        </div>
        <button type="submit" class="btn btn-primary">Iniciar sesión</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: '',
        password: ''
      };
    },
    methods: {
      login() {
        // Lógica de inicio de sesión aquí
        // Enviar datos al servidor, realizar validaciones, etc.
        console.log('Inicio de sesión:', this.email, this.password);
      }
    }
  };
  </script>
  