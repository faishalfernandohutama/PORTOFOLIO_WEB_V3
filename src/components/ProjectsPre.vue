<script setup>
import { Icon } from '@iconify/vue'
</script>

<template>
  <section class="grid gap-20 text-white px-6 py-12 max-w-7xl mx-auto">
    <div class="text-center space-y-4">
      <h1 class="text-4xl md:text-5xl lg:text-6xl font-changaOne uppercase tracking-wider">
        Selected Projects
      </h1>
      <p class="text-white/50 font-dmSans max-w-2xl mx-auto text-sm md:text-base">
        A collection of web applications and digital solutions I've built, focusing on efficiency,
        clean architecture, and seamless user experience.
      </p>
    </div>

    <div class="grid gap-16 md:gap-24 mt-8">
      <div class="group relative grid md:grid-cols-2 gap-8 md:gap-12 items-center">
        <div class="flex flex-col justify-center order-2 md:order-1 space-y-6">
          <div class="space-y-4">
            <h2
              class="uppercase text-3xl font-changaOne tracking-wide group-hover:text-purple-400 transition-colors duration-300"
            >
              Clipper Crafters
            </h2>
            <p class="text-white/60 font-dmSans leading-relaxed text-sm md:text-base">
              Web-based system for UMKM to manage bookings and customer interaction efficiently.
              Designed to streamline daily operations for local businesses.
            </p>
          </div>

          <div
            class="flex flex-wrap items-center justify-between gap-6 pt-4 border-t border-white/10"
          >
            <ul class="flex gap-3">
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="vscode-icons:file-type-html" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="vscode-icons:file-type-css" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:javascript" class="w-5 h-5" />
              </li>
            </ul>
            <a
              href="https://github.com/faishalfernandohutama/MbkmSkilvul"
              class="px-6 py-2.5 text-sm font-dmSans font-medium bg-white text-black rounded-full hover:bg-purple-500 hover:text-white transition-all duration-300 flex items-center gap-2"
            >
              View Github <Icon icon="mdi:arrow-top-right" class="w-4 h-4" />
            </a>
          </div>
        </div>
        <div
          class="relative overflow-hidden rounded-2xl aspect-video bg-white/5 border border-white/10 order-1 md:order-2"
        >
          <img
            src="./icons/clip.png"
            alt="Clipper Crafters"
            class="object-cover w-full h-full grayscale group-hover:grayscale-0 group-hover:scale-105 transition-all duration-700 ease-in-out"
          />
        </div>
      </div>

      <div class="group relative grid md:grid-cols-2 gap-8 md:gap-12 items-center">
        <div
          class="relative overflow-hidden rounded-2xl aspect-video bg-white/5 border border-white/10 order-1 md:order-1"
        >
          <img
            src="./icons/ERP.png"
            alt="ERP Project"
            class="object-cover w-full h-full grayscale group-hover:grayscale-0 group-hover:scale-105 transition-all duration-700 ease-in-out"
          />
        </div>
        <div class="flex flex-col justify-center order-2 md:order-2 space-y-6">
          <div class="space-y-4">
            <h2
              class="uppercase text-3xl font-changaOne tracking-wide group-hover:text-purple-400 transition-colors duration-300"
            >
              ERP Project
            </h2>
            <p class="text-white/60 font-dmSans leading-relaxed text-sm md:text-base">
              Full-Stack Enterprise Resource Planning (ERP) System designed to manage, automate, and
              integrate business operations. Built with a decoupled architecture featuring a
              responsive dashboard and a secure RESTful API backend handling complex business logic.
            </p>
          </div>

          <div
            class="flex flex-wrap items-center justify-between gap-6 pt-4 border-t border-white/10"
          >
            <ul class="flex gap-3">
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="simple-icons:express" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:react" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:tailwindcss-icon" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:nodejs-icon" class="w-5 h-5" />
              </li>
            </ul>
            <a
              href="https://github.com/ERPUas"
              class="px-6 py-2.5 text-sm font-dmSans font-medium bg-white text-black rounded-full hover:bg-purple-500 hover:text-white transition-all duration-300 flex items-center gap-2"
            >
              View Github <Icon icon="mdi:arrow-top-right" class="w-4 h-4" />
            </a>
          </div>
        </div>
      </div>

      <div class="group relative grid md:grid-cols-2 gap-8 md:gap-12 items-center">
        <div class="flex flex-col justify-center order-2 md:order-1 space-y-6">
          <div class="space-y-4">
            <h2
              class="uppercase text-3xl font-changaOne tracking-wide group-hover:text-purple-400 transition-colors duration-300"
            >
              CatBoost Prediction
            </h2>
            <p class="text-white/60 font-dmSans leading-relaxed text-sm md:text-base">
              Machine Learning Web Implementation for Plantation Production Prediction. A
              React-based dashboard covering an end-to-end workflow—from data preprocessing using
              the CatBoost algorithm to presenting optimized predictive models through a clean UI.
            </p>
          </div>

          <div
            class="flex flex-wrap items-center justify-between gap-6 pt-4 border-t border-white/10"
          >
            <ul class="flex gap-3">
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:python" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:react" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:tailwindcss-icon" class="w-5 h-5" />
              </li>
            </ul>
            <a
              href="https://github.com/faishalfernandohutama/Prediksi_Produksi"
              class="px-6 py-2.5 text-sm font-dmSans font-medium bg-white text-black rounded-full hover:bg-purple-500 hover:text-white transition-all duration-300 flex items-center gap-2"
            >
              View Github <Icon icon="mdi:arrow-top-right" class="w-4 h-4" />
            </a>
          </div>
        </div>
        <div
          class="relative overflow-hidden rounded-2xl aspect-video bg-white/5 border border-white/10 order-1 md:order-2"
        >
          <img
            src="./icons/cat.png"
            alt="CatBoost Prediction"
            class="object-cover w-full h-full grayscale group-hover:grayscale-0 group-hover:scale-105 transition-all duration-700 ease-in-out"
          />
        </div>
      </div>

      <div class="group relative grid md:grid-cols-2 gap-8 md:gap-12 items-center">
        <div
          class="relative overflow-hidden rounded-2xl aspect-video bg-white/5 border border-white/10 order-1 md:order-1"
        >
          <img
            src="./icons/InnHubb.png"
            alt="InnHub"
            class="object-cover w-full h-full grayscale group-hover:grayscale-0 group-hover:scale-105 transition-all duration-700 ease-in-out"
          />
        </div>
        <div class="flex flex-col justify-center order-2 md:order-2 space-y-6">
          <div class="space-y-4">
            <h2
              class="uppercase text-3xl font-changaOne tracking-wide group-hover:text-purple-400 transition-colors duration-300"
            >
              InnHub
            </h2>
            <p class="text-white/60 font-dmSans leading-relaxed text-sm md:text-base">
              Integrated Hospitality & Property Management System. A modern platform designed to
              simplify reservations and property operations, featuring real-time room data
              management and scalable API services.
            </p>
          </div>

          <div
            class="flex flex-wrap items-center justify-between gap-6 pt-4 border-t border-white/10"
          >
            <ul class="flex gap-3">
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="simple-icons:express" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:react" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:tailwindcss-icon" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:nodejs-icon" class="w-5 h-5" />
              </li>
            </ul>
            <a
              href="https://github.com/orgs/FullStack-7/repositories"
              class="px-6 py-2.5 text-sm font-dmSans font-medium bg-white text-black rounded-full hover:bg-purple-500 hover:text-white transition-all duration-300 flex items-center gap-2"
            >
              View Github <Icon icon="mdi:arrow-top-right" class="w-4 h-4" />
            </a>
          </div>
        </div>
      </div>

      <div class="group relative grid md:grid-cols-2 gap-8 md:gap-12 items-center">
        <div class="flex flex-col justify-center order-2 md:order-1 space-y-6">
          <div class="space-y-4">
            <h2
              class="uppercase text-3xl font-changaOne tracking-wide group-hover:text-purple-400 transition-colors duration-300"
            >
              CukurRans
            </h2>
            <p class="text-white/60 font-dmSans leading-relaxed text-sm md:text-base">
              Digital Barbershop Booking & Management System. Modernizing conventional services by
              allowing online appointments and efficient queue management. Built with a decoupled
              architecture for fast user-side performance.
            </p>
          </div>

          <div
            class="flex flex-wrap items-center justify-between gap-6 pt-4 border-t border-white/10"
          >
            <ul class="flex gap-3">
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="simple-icons:express" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:react" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:tailwindcss-icon" class="w-5 h-5" />
              </li>
              <li
                class="p-2.5 bg-white/5 rounded-lg border border-white/10 text-white/70 hover:text-white hover:bg-white/10 transition-all"
              >
                <Icon icon="logos:nodejs-icon" class="w-5 h-5" />
              </li>
            </ul>
            <a
              href="#"
              class="px-6 py-2.5 text-sm font-dmSans font-medium bg-white text-black rounded-full hover:bg-purple-500 hover:text-white transition-all duration-300 flex items-center gap-2"
            >
              View Github <Icon icon="mdi:arrow-top-right" class="w-4 h-4" />
            </a>
          </div>
        </div>
        <div
          class="relative overflow-hidden rounded-2xl aspect-video bg-white/5 border border-white/10 order-1 md:order-2"
        >
          <img
            src="./icons/Cukur.png"
            alt="CukurRans"
            class="object-cover w-full h-full grayscale group-hover:grayscale-0 group-hover:scale-105 transition-all duration-700 ease-in-out"
          />
        </div>
      </div>
    </div>

    <div class="mt-20 flex justify-center md:justify-end">
      <svg class="w-20 h-20 text-purple-400 animate-fadeIn" viewBox="0 0 100 100" fill="none">
        <path
          d="M20 20 C20 60, 80 40, 80 80"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          class="animate-draw"
        />
        <polyline
          points="70,75 80,85 90,75"
          stroke="currentColor"
          stroke-width="2"
          fill="none"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="animate-bounceArrow"
        />
      </svg>
    </div>
  </section>
</template>

<style>
/* Animasi Panah (Tetap dipertahankan dari kode Anda sebelumnya) */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.animate-fadeIn {
  animation: fadeIn 1s ease forwards;
}

@keyframes draw {
  from {
    stroke-dasharray: 200;
    stroke-dashoffset: 200;
  }
  to {
    stroke-dashoffset: 0;
  }
}
.animate-draw {
  stroke-dasharray: 200;
  stroke-dashoffset: 200;
  animation: draw 1.5s ease forwards;
}

@keyframes bounceArrow {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(6px);
  }
}
.animate-bounceArrow {
  animation: bounceArrow 1.5s infinite ease-in-out;
}
</style>
