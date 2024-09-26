<template>
  <div>
    <header>
      <div class="container">
        <h1 class="logo">Nuestro sitio web</h1>
        <nav>
          <ul>
            <li><router-link to="/">Inicio</router-link></li>
            <li><router-link to="/about">Acerca de Nuxt.js </router-link></li>
            <li><router-link to="/contact">Contactanos</router-link></li>
          </ul>
        </nav>
      </div>
    </header>

    <main>
      <section class="hero">
        <div class="container">
          <h2>Bienvenido a nuestro sitio web sobre Nuxt.js </h2>
          <p>Dale click en "empezar" y aprende un poco sobre esta herramienta</p>
          <router-link to="/about" class="cta-btn">Empezar</router-link>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2024 My Website. All rights reserved.</p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>

<style scoped>
/* General Styles */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #333;
}
.container {
  align-items: center;
  max-width: 1200px;
  margin: auto;
}

/* Header */
header {
  background: #333;
  color: #fff;
  padding: 30px 0;
}

.logo {
  float: left;
  font-size: 20px;
}

nav {
  float: right;
}

nav ul {
  list-style: none;
}

nav ul li {
  display: inline;
  margin-left: 40px;
}

nav ul li a {
  color: #fff;
  text-decoration: none;
  font-size: 18px;
}

nav ul li a:hover {
  color: #f4b400;
}

/* Hero Section */
.hero {
  background: url('https://images5.alphacoders.com/357/thumb-1920-357800.jpg');
  background-repeat: no-repeat;
  height: 550px;
  background-size: cover;
  display: flex;
  align-items: center;
  text-align: center;
}

.hero h2 {
  font-size: 48px;
  color: #fff;
}

.hero p {
  font-size: 18px;
  color: #f4f4f4;
  margin: 20px 0;
}

.cta-btn {
  display: inline-block;
  padding: 10px 20px;
  background: #f4b400;
  color: #fff;
  text-decoration: none;
  font-size: 18px;
  border-radius: 5px;
}

.cta-btn:hover {
  background: #d49600;
}

/* Footer */
footer {
  background: #333;
  color: #fff;
  text-align: center;
  padding: 40px 0;
}
</style>
