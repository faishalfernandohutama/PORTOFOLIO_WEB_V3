<script setup lang="ts">
import About from '@/components/About.vue'
import Contacts from '@/components/Contacts.vue'
import Header from '@/components/Header.vue'
import Hero from '@/components/Hero.vue'
import ProjectsPre from '@/components/ProjectsPre.vue'
</script>

<template>
  <div>
    <!-- HERO -->
    <section id="home" class="">
      <Hero />
      <Header />
    </section>

    <!-- ABOUT -->
    <section id="about" class="">
      <About />
    </section>

    <!-- PROJECT -->
    <section id="projects" class="min-h-screen">
      <ProjectsPre />
    </section>

    <!-- CONTACT -->
    <section id="contact" class="min-h-screen">
      <Contacts />
    </section>
  </div>
</template>

<style>
/* biar scroll ke anchor nggak ketutup navbar */
section {
  scroll-margin-top: 4rem; /* = h-16 */
}
</style>
