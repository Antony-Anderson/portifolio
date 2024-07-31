<script setup lang="ts">
import Apresentacao from './Apresentacao.vue';
import Footer from './Footer.vue';

</script>

<template>
  <div>
    <nav>
      <a href="#section1">Apresentação</a>
      <a href="#section2">Seção 2</a>
      <a href="#section3">Seção 3</a>
    </nav>

    <section id="section1" class="mt-4">
      <Apresentacao></Apresentacao>
    </section>

    <section id="section2">
      <h1>Seção 2</h1>
      <p>Conteúdo da Seção 2</p>
    </section>

    <section id="section3">
      <h1>Seção 3</h1>
      <p>Conteúdo da Seção 3</p>
    </section>
    <Footer></Footer>
  </div>
</template>

<style scoped>
  b   body {
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
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 14px 20px;
            display: inline-block;
            position: relative;
            transition: color 0.3s ease, transform 0.3s ease;
        }
        nav a::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 0;
            height: 2px;
            background-color: #ff5733;
            transition: width 0.3s ease;
        }
        nav a:hover {
            color: #ff5733;
            transform: scale(1.1);
        }
        nav a:hover::after {
            width: 100%;
        }
        section {
            padding: 100px;
            padding-top: 60px;
            height: 100vh;
        }
        #section1 { background-color: white; }
        #section2 { background-color: lightblue; }
        #section3 { background-color: lightgreen; }
</style>


