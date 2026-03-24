<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue'

const isOpen = ref(false)
const isScrolled = ref(false)
const isAtBottom = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50

  const scrollPosition = window.innerHeight + window.scrollY
  const documentHeight = document.documentElement.scrollHeight

  isAtBottom.value = scrollPosition >= documentHeight - 10
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
  handleScroll()
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<template>
  <div
    class="fixed bottom-0 left-0 right-0 h-32 z-40 pointer-events-none transition-all duration-500 ease-in-out"
    :class="isScrolled && !isAtBottom ? 'opacity-100' : 'opacity-0'"
  >
    <div
      class="absolute inset-0 backdrop-blur-[20px] [mask-image:linear-gradient(to_top,black_20%,transparent_100%)] [-webkit-mask-image:linear-gradient(to_top,black_20%,transparent_100%)]"
    ></div>
  </div>

  <div
    class="fixed bottom-8 left-1/2 -translate-x-1/2 z-[60] transition-all duration-500 ease-out"
    :class="isScrolled ? 'opacity-100 translate-y-0' : 'opacity-0 translate-y-10'"
  >
    <div
      class="flex items-center gap-6 px-6 py-3 rounded-full bg-white/5 backdrop-blur-md border border-white/20 shadow-lg text-white transition-all duration-500"
    >
      <a
        href="#home"
        class="flex items-center hover:opacity-80 transition-opacity"
        @click="isOpen = false"
      >
        <img src="./icons/logoPersonal.png" alt="My Logo" class="h-8 w-auto object-contain" />
      </a>

      <ul class="hidden md:flex gap-6 items-center border-l border-white/20 pl-6">
        <li>
          <a href="#skills" class="hover:text-purple-400 transition-colors cursor-pointer"
            >Skills</a
          >
        </li>
        <li>
          <a href="#about" class="hover:text-purple-400 transition-colors cursor-pointer">About</a>
        </li>
        <li>
          <a href="#projects" class="hover:text-purple-400 transition-colors cursor-pointer"
            >Projects</a
          >
        </li>
        <li>
          <a href="#contact" class="hover:text-purple-400 transition-colors cursor-pointer"
            >Contacts</a
          >
        </li>
      </ul>

      <button
        @click="isOpen = !isOpen"
        class="md:hidden relative w-6 h-6 flex items-center justify-center focus:outline-none ml-2"
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
      class="fixed inset-0 bg-black/95 backdrop-blur-2xl z-50 flex flex-col justify-center items-center text-white gap-8 text-2xl font-changaOne uppercase tracking-widest"
    >
      <a href="#home" @click="isOpen = false" class="hover:text-purple-400 transition-colors"
        >Home</a
      >
      <a href="#skills" @click="isOpen = false" class="hover:text-purple-400 transition-colors"
        >Skills</a
      >
      <a href="#about" @click="isOpen = false" class="hover:text-purple-400 transition-colors"
        >About</a
      >
      <a href="#projects" @click="isOpen = false" class="hover:text-purple-400 transition-colors"
        >Projects</a
      >
      <a href="#contact" @click="isOpen = false" class="hover:text-purple-400 transition-colors"
        >Contacts</a
      >
    </div>
  </transition>
</template>

<style>
/* Animasi Fade untuk menu mobile tetap sama */
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
