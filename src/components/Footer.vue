<script setup>
import { Icon } from '@iconify/vue'
</script>

<template>
  <footer class="min-h-screen relative overflow-hidden bg-black pt-32 pb-8 text-white">
    <div
      class="absolute top-10 left-0 w-full overflow-hidden flex justify-center select-none pointer-events-none opacity-30"
    >
      <h1
        class="text-[18vw] font-changaOne uppercase tracking-tighter whitespace-nowrap leading-none"
        style="-webkit-text-stroke: 2px white; color: transparent"
      >
        FAISHAL FERNANDO
      </h1>
    </div>

    <div class="relative z-10 w-full py-8 mt-12">
      <div class="flex whitespace-nowrap animate-marquee w-max select-none">
        <div
          class="flex items-center gap-6 px-4 text-4xl md:text-6xl lg:text-7xl font-changaOne tracking-wide"
        >
          <span>Let's work together</span>
          <Icon icon="mdi:asterisk" class="w-10 h-10 md:w-12 md:h-12 text-purple-500" />
          <span>Let's work together</span>
          <Icon icon="mdi:asterisk" class="w-10 h-10 md:w-12 md:h-12 text-purple-500" />
          <span>Let's work together</span>
          <Icon icon="mdi:asterisk" class="w-10 h-10 md:w-12 md:h-12 text-purple-500" />
        </div>
        <div
          class="flex items-center gap-6 px-4 text-4xl md:text-6xl lg:text-7xl font-changaOne tracking-wide"
        >
          <span>Let's work together</span>
          <Icon icon="mdi:asterisk" class="w-10 h-10 md:w-12 md:h-12 text-purple-500" />
          <span>Let's work together</span>
          <Icon icon="mdi:asterisk" class="w-10 h-10 md:w-12 md:h-12 text-purple-500" />
          <span>Let's work together</span>
          <Icon icon="mdi:asterisk" class="w-10 h-10 md:w-12 md:h-12 text-purple-500" />
        </div>
      </div>
    </div>

    <div class="relative z-10 mt-16 flex flex-col items-center gap-4 font-dmSans text-white/80">
      <a
        href="mailto:nandolop71@gmail.com"
        class="flex items-center gap-3 text-lg md:text-xl hover:text-purple-400 transition-colors duration-300"
      >
        <Icon icon="mdi:email" class="w-5 h-5 md:w-6 md:h-6" />
        nandolop71@gmail.com
      </a>
      <p class="flex items-center gap-3 text-lg md:text-xl">
        <Icon icon="mdi:map-marker" class="w-5 h-5 md:w-6 md:h-6" />
        Sidoarjo, East Java
      </p>

      <div class="flex items-center gap-6 mt-4">
        <a
          href="https://github.com/faishalfernandohutama"
          target="_blank"
          rel="noopener noreferrer"
          class="p-2 bg-white/5 border border-white/10 rounded-full hover:bg-white/10 hover:text-purple-400 hover:scale-110 transition-all duration-300"
        >
          <Icon icon="mdi:github" class="w-6 h-6 md:w-7 md:h-7" />
        </a>
        <a
          href="https://www.linkedin.com/in/faishalfernando"
          target="_blank"
          rel="noopener noreferrer"
          class="p-2 bg-white/5 border border-white/10 rounded-full hover:bg-white/10 hover:text-purple-400 hover:scale-110 transition-all duration-300"
        >
          <Icon icon="mdi:linkedin" class="w-6 h-6 md:w-7 md:h-7" />
        </a>
      </div>
    </div>

    <div
      class="relative z-10 mt-32 px-6 max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-4 text-xs md:text-sm text-white/40 font-dmSans"
    >
      <p>&copy; 2026 Faishal Fernando</p>

      <div class="flex items-center gap-2">
        <span>Built with</span>
        <div class="flex gap-2 ml-1">
          <Icon
            icon="logos:vue"
            class="w-4 h-4 md:w-5 md:h-5 grayscale opacity-60 hover:grayscale-0 hover:opacity-100 transition-all duration-300"
          />
          <Icon
            icon="logos:tailwindcss-icon"
            class="w-4 h-4 md:w-5 md:h-5 grayscale opacity-60 hover:grayscale-0 hover:opacity-100 transition-all duration-300"
          />
        </div>
      </div>

      <p>All rights reserved.</p>
    </div>
  </footer>
</template>

<style>
@keyframes marquee {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(-50%);
  }
}

.animate-marquee {
  animation: marquee 20s linear infinite;
}
</style>
