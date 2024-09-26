<template>
    <div class="background">
      <div>
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
  
        <div class="about-container">
          <h1>¿Qué es Nuxt.js?</h1>
          <p>Nuxt.js es un framework basado en Vue.js que simplifica el desarrollo de aplicaciones web universales y estáticas. Permite crear aplicaciones que pueden ser renderizadas tanto del lado del servidor (SSR) como del lado del cliente, mejorando el rendimiento y la experiencia del usuario.</p>
          
          <h2>Características Clave</h2>
          <ul>
            <li><strong>Renderizado del lado del servidor (SSR):</strong> Mejora el SEO y el tiempo de carga inicial al renderizar el contenido en el servidor.</li>
            <li><strong>Generación de sitios estáticos:</strong> Crea sitios completamente estáticos que se pueden desplegar fácilmente en cualquier servidor.</li>
            <li><strong>Soporte para módulos:</strong> Amplía las funcionalidades con módulos de terceros para mejorar la productividad.</li>
            <li><strong>Facilidad de configuración:</strong> Ofrece una configuración mínima para que puedas empezar rápidamente con tu proyecto.</li>
          </ul>
  
          <p>En resumen, Nuxt.js es una excelente opción para desarrolladores que buscan construir aplicaciones robustas y optimizadas con Vue.js.</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AboutPage'
  }
  </script>
  
  <style scoped>
  /* Fondo de la página */
  .background {
    background-image: url('https://images5.alphacoders.com/357/thumb-1920-357800.jpg'); /* Imagen de fondo */
    background-size: cover;
    background-position: center;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
  }
  
  /* Barra de navegación */
  header {
  background: #333;
  color: #fff;
  padding: 30px 0;
  
}
  
  .container {
  align-items: center;
  max-width: 1200px;
  margin: auto;
  }
  
  .logo {
  float: left;
  font-size: 20px;
  color: #fff;
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
    color: #f3f2f2;
  }
  
  /* Estilos del contenido */
  .about-container {
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
  
  h2 {
    font-size: 1.8rem;
    color: #444;
    margin-top: 30px;
    margin-bottom: 10px;
    border-bottom: 2px solid #e0dfdd; 
    padding-bottom: 5px;
  }
  
  p {
    font-size: 1.2rem;
    color: #666;
    margin-top: 10px;
    line-height: 1.6;
  }
  
  ul {
    margin-top: 10px;
    list-style-type: disc;
    padding-left: 20px;
  }
  
  li {
    font-size: 1.1rem;
    color: #4e4b4b;
    margin-bottom: 5px;
    position: relative;
  }
  
  li::marker {
    color: #f4b400;
  }
  
  li:hover {
    background-color: #f4b400;
    border-radius: 5px;
    padding: 5px;
  }
  </style>
  