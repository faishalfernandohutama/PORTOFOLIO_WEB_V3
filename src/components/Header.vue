<script setup lang="ts">
import { ref } from 'vue'

const isOpen = ref(false)
</script>

<template>
  <!-- NAVBAR -->
  <header
    class="absolute top-0 left-0 w-full h-16 flex items-center justify-between px-8 py-14 md:px-20 z-50"
  >
    <!-- Logo -->
    <button class="h-16 flex items-center">
      <img src="./icons/logoPersonal.png" alt="Logo" class="h-full object-contain" />
    </button>

    <!-- Hamburger -->
    <button
      @click="isOpen = !isOpen"
      class="md:hidden relative w-10 h-10 flex items-center justify-center"
    >
      <!-- garis atas -->
      <span
        class="absolute w-6 h-0.5 bg-white transition-all duration-300"
        :class="isOpen ? 'rotate-45' : '-translate-y-2'"
      ></span>

      <!-- garis tengah -->
      <span
        class="absolute w-6 h-0.5 bg-white transition-all duration-300"
        :class="isOpen ? 'opacity-0' : ''"
      ></span>

      <!-- garis bawah -->
      <span
        class="absolute w-6 h-0.5 bg-white transition-all duration-300"
        :class="isOpen ? '-rotate-45' : 'translate-y-2'"
      ></span>
    </button>

    <!-- Desktop Menu -->
    <ul class="hidden md:flex gap-8 text-white">
      <li class="cursor-pointer">About</li>
      <li class="cursor-pointer">Contacts</li>
      <li class="cursor-pointer">Projects</li>
    </ul>
  </header>

  <!-- SPACER (biar konten tidak ketutup navbar fixed) -->
  <div class="h-16"></div>

  <!-- MOBILE FULLSCREEN MENU -->
  <transition name="fade">
    <div
      v-if="isOpen"
      class="fixed inset-0 bg-darkBlue z-40 flex flex-col justify-center text-white items-center gap-8 text-xl"
    >
      <a href="#about" @click="isOpen = false">About</a>
      <a href="#contact" @click="isOpen = false">Contacts</a>
      <a href="#projects" @click="isOpen = false">Projects</a>
    </div>
  </transition>
</template>

<style>
/* Smooth fade */
.fade-enter-from {
  opacity: 0;
}
.fade-enter-to {
  opacity: 1;
}
.fade-enter-active {
  transition: opacity 0.3s ease;
}

.fade-leave-from {
  opacity: 1;
}
.fade-leave-to {
  opacity: 0;
}
.fade-leave-active {
  transition: opacity 0.2s ease;
}

/* Hindari scroll aneh */
body {
  overflow-x: hidden;
}
</style>
