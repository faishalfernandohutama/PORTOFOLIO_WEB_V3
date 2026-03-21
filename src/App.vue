<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="bg-black">
    <header>
      <RouterView />
      <Footer />
    </header>
  </div>
</template>
