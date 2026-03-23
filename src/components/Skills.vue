<script setup>
import { ref } from 'vue'

// Data FAQ
const faqs = ref([
  {
    q: 'What is your primary specialization as a Web Developer ?',
    a: 'I am a Full-Stack Developer specializing in building scalable, responsive, and high-performance web applications. My core expertise lies in the MERN Stack (MongoDB, Express, React, Node.js) and Vue.js. Additionally, I am highly proficient in backend development using PHP (CodeIgniter 4) and Python for data-driven solutions.',
  },
  {
    q: 'Why should I hire a Fresh Graduate for my project ?',
    a: 'As a fresh graduate, I bring high energy, a deep understanding of the latest tech trends, and a commitment to delivering top-tier results to build my professional reputation. I offer modern, clean-code solutions with a focus on efficiency and long-term maintainability.',
  },
  {
    q: 'Which framework do you recommend for large-scale applications ?',
    a: 'For applications requiring high performance and real-time capabilities, I recommend the MERN Stack eather use Vue or React or you can change a database like mySql/mariaDB or whatever u like. However, if your project requires structured data management with a robust PHP ecosystem, I am an expert at implementing CodeIgniter 4 to ensure speed and security.',
  },
  {
    q: 'Can you convert designs from Figma or Adobe XD into functional code ?',
    a: 'Absolutely. I have a strong eye for detail and can translate visual designs into pixel-perfect, responsive interfaces using Tailwind CSS. I ensure that the user experience remains consistent and fluid across all device sizes.',
  },
  {
    q: 'How do you ensure the application is bug-free and reliable ?',
    a: 'I follow a systematic development process: starting with clear architecture planning, writing code following Clean Code principles, and performing internal testing. I also maintain an open feedback loop for revisions to ensure the final product aligns perfectly with your requirements.',
  },
  {
    q: 'Can you integrate data analysis or predictive models into a website ?',
    a: 'Yes, I can. With my background in Data Science and Machine Learning (specifically using Gradient Boosting methods like CatBoost), I can build and integrate smart analytical features or predictive models into your web dashboard using Python-based APIs.',
  },
])

// State untuk menyimpan index yang sedang terbuka
const activeIndex = ref(null)

const toggleFaq = (index) => {
  activeIndex.value = activeIndex.value === index ? null : index
}
</script>

<template>
  <section class="min-h-screen grid content-start gap-10 text-white px-6 py-20 max-w-7xl mx-auto">
    <div class="space-y-4">
      <h3 class="text-sm font-dmSans text-gray-400">Common questions and answers</h3>
      <h1 class="text-4xl md:text-5xl font-dmSans leading-tight">
        Frequently Asked <span class="text-yellow-200">Questions</span>
      </h1>
    </div>

    <div class="space-y-4">
      <div
        v-for="(faq, index) in faqs"
        :key="index"
        @click="toggleFaq(index)"
        class="card-clean relative border border-white/10 rounded-2xl p-6 cursor-pointer group transition-all duration-300 hover:bg-white/5"
      >
        <div class="flex justify-between items-center gap-4">
          <p class="font-medium text-lg">{{ faq.q }}</p>

          <div class="relative w-6 h-6 flex items-center justify-center">
            <div class="absolute w-4 h-0.5 bg-white transition-transform duration-300"></div>
            <div
              class="absolute w-4 h-0.5 bg-white transition-transform duration-300"
              :class="activeIndex === index ? 'rotate-0' : 'rotate-90'"
            ></div>
          </div>
        </div>

        <div
          class="grid transition-all duration-300 ease-in-out"
          :class="
            activeIndex === index ? 'grid-rows-[1fr] opacity-100 mt-4' : 'grid-rows-[0fr] opacity-0'
          "
        >
          <div class="overflow-hidden text-white/70 leading-relaxed">
            {{ faq.a }}
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Efek Border Gradient */
.card-clean::before {
  content: '';
  position: absolute;
  inset: 0;
  padding: 1.5px;
  border-radius: inherit;
  background: linear-gradient(
    120deg,
    rgba(0, 255, 255, 0.2),
    rgba(139, 92, 246, 0.2),
    rgba(236, 72, 153, 0.2)
  );
  -webkit-mask:
    linear-gradient(#fff 0 0) content-box,
    linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
  mask-composite: exclude;
  pointer-events: none;
}

/* Glow Effect saat Hover */
.card-clean:hover::after {
  content: '';
  position: absolute;
  inset: -2px;
  border-radius: inherit;
  background: linear-gradient(
    120deg,
    rgba(0, 255, 255, 0.1),
    rgba(139, 92, 246, 0.1),
    rgba(236, 72, 153, 0.1)
  );
  filter: blur(15px);
  opacity: 0.6;
  z-index: -1;
}
</style>
