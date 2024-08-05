<script setup lang="ts">
import Apresentacao from './Apresentacao.vue';
import Footer from './Footer.vue';
import Formacoes from './Formacoes.vue';
import Linguagens from './Linguagens.vue';
import Portifolio from './Portifolio.vue';
import { ref } from 'vue';

const isMenuOpen = ref(false);
const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};
</script>

<template>
  <div>
    <nav>
      <button class="menu-toggle" @click="toggleMenu">
        <span class="menu-icon">&#9776;</span>
      </button>
      <div :class="{ 'nav-links': true, 'active': isMenuOpen }">
        <a href="#section1">Apresentação</a>
        <a href="#section2">Formações e cursos</a>
        <a href="#section3">Portifólio</a>
        <a href="#section4">Linguagens e frameworks</a>
        <a href="#section5">Fale comigo</a>
      </div>
    </nav>

    <section id="section1" class="section">
      <Apresentacao></Apresentacao>
    </section>

    <section id="section2" class="section">
      <Formacoes></Formacoes>
    </section>

    <section id="section3" class="section">
      <Portifolio></Portifolio>
    </section>

    <section id="section4" class="section">
      <Linguagens></Linguagens>
    </section>
    
    <section id="section5" class="footer-section">
      <Footer></Footer>
    </section>
  </div>
</template>

<style scoped>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    scroll-behavior: smooth;
  }

  nav {
    background-color: #333;
    padding: 10px 20px;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
    display: flex;
    align-items: center;
    box-sizing: border-box;
    justify-content: space-between;
  }

  .menu-toggle {
    background: none;
    border: none;
    color: white;
    font-size: 24px;
    cursor: pointer;
    display: none;
  }

  .menu-icon {
    display: inline-block;
  }

  .nav-links {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
  }

  .nav-links a {
    color: white;
    text-decoration: none;
    padding: 14px 20px;
    display: inline-block;
    position: relative;
    transition: color 0.3s ease, transform 0.3s ease;
  }

  .nav-links a::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    width: 0;
    height: 2px;
    background-color: #ff5733;
    transition: width 0.3s ease;
  }

  .nav-links a:hover {
    color: #ff5733;
    transform: scale(1.1);
  }

  .nav-links a:hover::after {
    width: 100%;
  }

  .section {
    padding: 50px;
    padding-top: 60px;
    min-height: 100vh;
  }

  #section1 { background-color: #1e1e1e; }
  #section2 { background-color: #181818; } 
  #section3 { background-color: #1e1e1e; }
  #section4 { background-color: #181818; }
  #section5 { background-color: #1e1e1e; }

  .footer-section {
    padding: 20px;
    background-color: #1e1e1e;
    min-height: 100px;
  }

  /* Responsividade */
  @media (max-width: 768px) {
    .nav-links {
      display: none;
      flex-direction: column;
      width: 100%;
      background-color: #333;
      position: absolute;
      top: 60px;
      left: 0;
    }

    .nav-links.active {
      display: flex;
    }

    .menu-toggle {
      display: block;
    }

    .nav-links a {
      padding: 10px;
      font-size: 0.9em;
    }

    .section {
      padding: 30px;
      padding-top: 70px;
    }
  }

  @media (max-width: 480px) {
    .nav-links a {
      padding: 8px;
      font-size: 0.8em;
    }

    .section {
      padding: 20px;
      padding-top: 80px;
    }

    .footer-section {
      padding: 15px;
      min-height: 80px;
    }
  }
</style>
