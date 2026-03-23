<template>
  <section
    ref="sectionRef"
    class="min-h-screen flex items-center justify-center bg-black max-w-7xl mx-auto overflow-hidden"
  >
    <h1
      class="font-dmSans text-2xl px-4 md:text-4xl lg:text-6xl text-center flex flex-wrap justify-center gap-x-4 gap-y-2 transition-transform duration-700 ease-out"
      :style="{ transform: `translate(${parallaxX}px, ${parallaxY}px)` }"
    >
      <span
        v-for="(word, index) in words"
        :key="index"
        class="transition-colors duration-700 ease-in-out"
        :class="isVisible ? 'text-white' : 'text-neutral-800'"
        :style="{ transitionDelay: `${index * 80}ms` }"
      >
        {{ word }}
      </span>
    </h1>
  </section>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const quote =
  'Transforming visions into high-performance web solutions. I streamline the development process to focus on what truly matters: efficiency and execution. I don’t just deliver code; I deliver ready-to-scale products that work.'
const words = quote.split(' ')

// State untuk Observer (Warna Teks)
const sectionRef = ref(null)
const isVisible = ref(false)
let observer

// State untuk Parallax Mouse
const parallaxX = ref(0)
const parallaxY = ref(0)

// Fungsi kalkulasi posisi kursor
const handleMouseMove = (e) => {
  // Menghitung jarak kursor dari titik tengah layar
  // Dibagi 40 untuk menentukan intensitas efek. Semakin besar angkanya, pergerakannya semakin halus/kecil.
  const x = (window.innerWidth / 2 - e.clientX) / 40
  const y = (window.innerHeight / 2 - e.clientY) / 40

  parallaxX.value = x
  parallaxY.value = y
}

onMounted(() => {
  // 1. Intersection Observer untuk mendeteksi scroll (Efek fade-in warna)
  observer = new IntersectionObserver(
    (entries) => {
      if (entries[0].isIntersecting) {
        isVisible.value = true
      } else {
        isVisible.value = false
      }
    },
    {
      threshold: 0.2,
    },
  )

  if (sectionRef.value) {
    observer.observe(sectionRef.value)
  }

  // 2. Menambahkan pendeteksi pergerakan mouse untuk Parallax
  window.addEventListener('mousemove', handleMouseMove)
})

onUnmounted(() => {
  // Membersihkan memori saat pengguna berpindah halaman
  if (observer && sectionRef.value) {
    observer.unobserve(sectionRef.value)
  }
  window.removeEventListener('mousemove', handleMouseMove)
})
</script>
