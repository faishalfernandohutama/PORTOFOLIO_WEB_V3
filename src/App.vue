<script setup lang="ts">
import { onMounted, onUnmounted } from 'vue'
import { RouterView } from 'vue-router'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Lenis from '@studio-freight/lenis'

let lenis: any

onMounted(() => {
  lenis = new Lenis({
    duration: 1.2,
    smoothWheel: true,
  })

  const raf = (time: number) => {
    lenis.raf(time)
    requestAnimationFrame(raf)
  }

  requestAnimationFrame(raf)
})

onUnmounted(() => {
  lenis?.destroy()
})
</script>

<template>
  <div class="bg-black text-white">
    <!-- CONTENT -->
    <main>
      <RouterView />
    </main>

    <!-- FOOTER -->
    <Footer />
  </div>
</template>
