<template>
  <section
    ref="sectionRef"
    class="min-h-screen flex items-center justify-center bg-black max-w-7xl mx-auto"
  >
    <h1
      class="font-dmSans text-4xl md:text-6xl text-center flex flex-wrap justify-center gap-x-4 gap-y-2"
    >
      <span
        v-for="(word, index) in words"
        :key="index"
        class="transition-colors duration-700 ease-in-out,"
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
const sectionRef = ref(null)
const isVisible = ref(false)
let observer

onMounted(() => {
  // Intersection Observer untuk mendeteksi scroll
  observer = new IntersectionObserver(
    (entries) => {
      // Jika elemen masuk ke dalam viewport (layar)
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
})

onUnmounted(() => {
  if (observer && sectionRef.value) {
    observer.unobserve(sectionRef.value)
  }
})
</script>
