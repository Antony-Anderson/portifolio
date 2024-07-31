<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Index from './components/Index.vue'

</script>

<template>
  <header>
    <Index></Index>
  </header>

  <RouterView />
</template>