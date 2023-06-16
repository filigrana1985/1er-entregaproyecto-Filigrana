<template>
    <div>
      <h2>Registro</h2>
      <form @submit.prevent="register">
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email" v-model="email" class="form-control" required>
        </div>
        <div class="form-group">
          <label for="password">Contraseña:</label>
          <input type="password" id="password" v-model="password" class="form-control" required>
        </div>
        <button type="submit" class="btn btn-primary">Registrarse</button>
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
      register() {
        // Lógica de registro aquí
        // Enviar datos al servidor, realizar validaciones, etc.
        console.log('Registro:', this.email, this.password);
      }
    }
  };
  </script>
  