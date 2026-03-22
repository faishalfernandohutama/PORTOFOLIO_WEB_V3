<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue'

const isOpen = ref(false)
const isScrolled = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<template>
  <div
    class="fixed bottom-0 left-0 right-0 h-32 z-40 pointer-events-none transition-all duration-500 ease-in-out"
    :class="isScrolled ? 'opacity-100' : 'opacity-0'"
  >
    <div
      class="absolute inset-0 backdrop-blur-[20px] [mask-image:linear-gradient(to_top,black_20%,transparent_100%)] [-webkit-mask-image:linear-gradient(to_top,black_20%,transparent_100%)]"
    ></div>
  </div>

  <div
    class="fixed bottom-8 left-1/2 -translate-x-1/2 z-50 transition-all duration-500 ease-out"
    :class="isScrolled ? 'opacity-100 translate-y-0' : 'opacity-0 translate-y-10'"
  >
    <div
      class="flex items-center gap-6 px-7 py-3 rounded-full bg-white/5 backdrop-blur-md border border-white/20 shadow-lg text-white"
    >
      <ul class="hidden md:flex gap-6 items-center">
        <li class="hover:text-gray-300 transition-colors cursor-pointer">Home</li>
        <li class="hover:text-gray-300 transition-colors cursor-pointer">Skills</li>
        <li class="hover:text-gray-300 transition-colors cursor-pointer">About</li>
        <li class="hover:text-gray-300 transition-colors cursor-pointer">Projects</li>
        <li class="hover:text-gray-300 transition-colors cursor-pointer">Contacts</li>
      </ul>

      <button
        @click="isOpen = !isOpen"
        class="md:hidden relative w-8 h-8 flex items-center justify-center focus:outline-none"
      >
        <span
          class="absolute w-5 h-0.5 bg-white transition-all duration-300"
          :class="isOpen ? 'rotate-45' : '-translate-y-1.5'"
        ></span>
        <span
          class="absolute w-5 h-0.5 bg-white transition-all duration-300"
          :class="isOpen ? 'opacity-0' : ''"
        ></span>
        <span
          class="absolute w-5 h-0.5 bg-white transition-all duration-300"
          :class="isOpen ? '-rotate-45' : 'translate-y-1.5'"
        ></span>
      </button>
    </div>
  </div>

  <transition name="fade">
    <div
      v-if="isOpen"
      class="fixed inset-0 bg-black/80 backdrop-blur-xl z-50 flex flex-col justify-center items-center text-white gap-8 text-xl"
    >
      <a href="#home" @click="isOpen = false" class="hover:text-gray-300">Home</a>
      <a href="#skills" @click="isOpen = false" class="hover:text-gray-300">Skills</a>
      <a href="#about" @click="isOpen = false" class="hover:text-gray-300">About</a>
      <a href="#projects" @click="isOpen = false" class="hover:text-gray-300">Projects</a>
      <a href="#contact" @click="isOpen = false" class="hover:text-gray-300">Contacts</a>
    </div>
  </transition>
</template>

<style>
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
</style>
