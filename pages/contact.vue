<template>
    <div class="background">
      <header>
        <div class="container">
          <h1 class="logo">Nuestro sitio web</h1>
          <nav>
            <ul>
              <li><router-link to="/">Inicio</router-link></li>
              <li><router-link to="/about">Acerca de Nuxt.js</router-link></li>
              <li><router-link to="/contact">Contáctanos</router-link></li>
            </ul>
          </nav>
        </div>
      </header>
  
      <div class="contact-container">
        <h1>Contáctanos</h1>
        <p>Si tienes alguna pregunta o comentario, no dudes en ponerte en contacto con nosotros. Completa el siguiente formulario y nos comunicaremos contigo a la brevedad.</p>
  
        <form @submit.prevent="handleSubmit">
          <div class="form-group">
            <label for="name">Nombre:</label>
            <input type="text" id="name" v-model="name" required />
          </div>
          <div class="form-group">
            <label for="email">Correo Electrónico:</label>
            <input type="email" id="email" v-model="email" required />
          </div>
          <div class="form-group">
            <label for="message">Mensaje:</label>
            <textarea id="message" v-model="message" rows="4" required></textarea>
          </div>
          <button type="submit">Enviar</button>
        </form>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ContactPage',
    data() {
      return {
        name: '',
        email: '',
        message: ''
      };
    },
    methods: {
      handleSubmit() {
        // Lógica para manejar el envío del formulario (ej. enviar a un API)
        console.log('Nombre:', this.name);
        console.log('Correo:', this.email);
        console.log('Mensaje:', this.message);
        // Resetea el formulario después de enviarlo
        this.name = '';
        this.email = '';
        this.message = '';
        alert('Gracias por tu mensaje! Nos pondremos en contacto pronto.');
      }
    }
  }
  </script>
  
  <style scoped>
  .background {
    background-image: url('https://images5.alphacoders.com/357/thumb-1920-357800.jpg'); /* Cambia a tu imagen */
    background-size: cover;
    background-position: center;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
  }
  
  header {
    background: #333;
    color: #fff;
    padding: 20px 0;
  }
  
  .container {
    max-width: 1200px;
    margin: auto;
    padding: 0 20px;
  }
  
  .logo {
    float: left;
    font-size: 24px;
  }
  
  nav {
    float: right;
  }
  
  nav ul {
    list-style: none;
  }
  
  nav ul li {
    display: inline;
    margin-left: 30px;
  }
  
  nav ul li a {
    color: #fff;
    text-decoration: none;
    font-size: 18px;
  }
  
  nav ul li a:hover {
    color: #f4b400;
  }
  
  .contact-container {
    max-width: 800px;
    margin: 50px auto;
    padding: 20px;
    background: rgba(255, 255, 255, 0.9);
    border-radius: 10px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  }
  
  h1 {
    font-size: 2.5rem;
    color: #333;
    text-align: center;
    margin-bottom: 20px;
  }
  
  p {
    font-size: 1.2rem;
    color: #666;
    text-align: center;
    margin-bottom: 30px;
  }
  
  .form-group {
    margin-bottom: 20px;
  }
  
  label {
    display: block;
    margin-bottom: 5px;
    color: #444;
  }
  
  input, textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 1rem;
  }
  
  button {
    background-color: #f4b400;
    color: #fff;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
  }
  
  button:hover {
    background-color: #d49600;
  }
  </style>
  