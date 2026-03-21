<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue'
import Header from './Header.vue'

const now = ref(new Date())
let interval: number

onMounted(() => {
  interval = setInterval(() => {
    now.value = new Date()
  }, 1000) // update tiap 1 detik
})

onUnmounted(() => {
  clearInterval(interval)
})
</script>

<template>
  <div class="relative h-screen w-full overflow-hidden text-white">
    <!-- 🎥 VIDEO -->
    <video
      class="absolute inset-0 w-full h-full object-cover z-0"
      src="./238264_medium.mp4"
      autoplay
      muted
      loop
      playsinline
    ></video>

    <!-- 🌑 OVERLAY GELAP -->
    <div class="absolute inset-0 bg-black/40 z-10"></div>

    <!-- 🔥 FADE BOTTOM -->
    <div
      class="absolute bottom-0 left-0 w-full h-64 z-20 bg-gradient-to-b from-transparent via-black/40 to-black pointer-events-none"
    ></div>

    <!-- 🌑 OVERLAY (biar teks kebaca) -->
    <div class="absolute inset-0 bg-black/40 md:bg-black/30 z-10"></div>

    <!-- 🧠 CONTENT -->
    <div
      class="relative z-20 flex flex-col items-center justify-center text-center px-4 gap-6 h-full"
    >
      <!-- top badge -->
      <div class="flex items-center gap-2 md:gap-4 tracking-wide">
        <p class="text-[10px] md:text-xs uppercase opacity-60">Site of the day</p>

        <h1
          class="border border-white/20 px-3 md:px-4 py-1 rounded-full text-[10px] md:text-xs backdrop-blur-sm bg-white/5"
        >
          {{
            now.toLocaleDateString('id-ID', {
              day: 'numeric',
              month: 'short',
              year: 'numeric',
            })
          }}
        </h1>

        <p class="text-[10px] md:text-xs opacity-60">Score 7.32 of 10</p>
      </div>

      <!-- title -->
      <h1 class="text-4xl md:text-6xl font-changaOne leading-tight tracking-wide">PORTOFOLIO</h1>

      <!-- subtitle -->
      <h2 class="text-sm md:text-xl font-changaOne opacity-90">Faishal Fernando Hutama</h2>
    </div>

    <!-- ⬇️ SCROLL INDICATOR -->
    <div class="scroll-indicator z-30 text-white opacity-80">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="w-8 h-8"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        stroke-width="2"
      >
        <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" />
      </svg>
    </div>
  </div>
</template>

<style scoped>
@keyframes floatDown {
  0%,
  100% {
    transform: translate(-50%, 0);
  }
  50% {
    transform: translate(-50%, 12px);
  }
}
.scroll-indicator {
  position: absolute;
  bottom: 30px;
  left: 50%;
  animation: floatDown 2s ease-in-out infinite;
}
</style>
