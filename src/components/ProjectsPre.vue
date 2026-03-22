<script setup>
import { Icon } from '@iconify/vue'
</script>

<template>
  <section class="grid gap-16 text-white px-6 max-w-7xl mx-auto">
    <!-- TITLE -->
    <div class="text-center">
      <h1 class="text-3xl font-changaOne md:text-4xl lg:text-6xl">EVERYTHING ABOUT MY PROJECT</h1>
    </div>

    <!-- CARD LIST -->
    <div class="grid gap-12">
      <!-- ================= CARD 1 ================= -->
      <div class="card-clean grid md:grid-cols-2 gap-10 items-center p-8 rounded-2xl">
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-semibold">Clipper Crafters</h2>
            <p class="text-gray-400 font-dmSans">
              Web-based system for UMKM to manage bookings and customer interaction.
            </p>
          </div>

          <div class="flex justify-between mt-6">
            <ul class="flex gap-3">
              <li class="icon-box"><Icon icon="vscode-icons:file-type-html" /></li>
              <li class="icon-box"><Icon icon="vscode-icons:file-type-css" /></li>
              <li class="icon-box"><Icon icon="logos:javascript" /></li>
            </ul>
            <button class="btn-clean">Github</button>
          </div>
        </div>

        <div class="image-box">
          <img src="./icons/clip.png" />
        </div>
      </div>

      <!-- ================= CARD 2 ================= -->
      <div class="card-clean grid md:grid-cols-2 gap-10 items-center p-8 rounded-2xl">
        <div class="image-box order-1 md:order-none">
          <img src="./icons/ERP.png" />
        </div>

        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-semibold">ERP Project</h2>
            <p class="text-gray-400 font-dmSans">
              Machine Learning Web Implementation: Plantation Production Predictor A React-based web
              application that functions as a plantation production prediction dashboard. This
              project covers an end-to-end workflow, from data preprocessing using the CatBoost
              algorithm to presenting results through a responsive user interface. The project's
              primary focus is predictive model optimization and user experience (UX) for monitoring
              agricultural production trends.
            </p>
          </div>

          <div class="flex justify-between mt-6">
            <ul class="flex gap-3">
              <li class="icon-box"><Icon icon="simple-icons:express" /></li>
              <li class="icon-box"><Icon icon="logos:react" /></li>
              <li class="icon-box"><Icon icon="logos:tailwindcss-icon" /></li>
              <li class="icon-box"><Icon icon="logos:nodejs-icon" /></li>
            </ul>
            <button class="btn-clean">Github</button>
          </div>
        </div>
      </div>

      <!-- ================= CARD 3 ================= -->
      <div class="card-clean grid md:grid-cols-2 gap-10 items-center p-8 rounded-2xl">
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-semibold">CatBoost Prediction</h2>
            <p class="text-gray-400 font-dmSans">
              Full-Stack Enterprise Resource Planning (ERP) System: A web-based ERP system designed
              to manage, automate, and integrate various business operational processes. This
              project is built with a decoupled architecture: The frontend repository focuses on a
              responsive and interactive dashboard interface, while the backend repository handles
              complex business logic, database management, and provides a secure RESTful API.
            </p>
          </div>

          <div class="flex justify-between mt-6">
            <ul class="flex gap-3">
              <li class="icon-box"><Icon icon="logos:python" /></li>
              <li class="icon-box"><Icon icon="logos:react" /></li>
              <li class="icon-box"><Icon icon="logos:tailwindcss-icon" /></li>
            </ul>
            <button class="btn-clean">Github</button>
          </div>
        </div>

        <div class="image-box">
          <img src="./icons/cat.png" />
        </div>
      </div>

      <!-- ================= CARD 4 ================= -->
      <div class="card-clean grid md:grid-cols-2 gap-10 items-center p-8 rounded-2xl">
        <div class="image-box order-1 md:order-none">
          <img src="./icons/InnHubb.png" />
        </div>

        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-semibold">InnHub</h2>
            <p class="text-gray-400 font-dmSans">
              InnHub: Integrated Hospitality & Property Management System InnHub is a modern lodging
              management platform designed to simplify the reservation process and property
              operations. Built on a full-stack architecture that separates the client and server
              sides, the application enables real-time management of room data, guest reservations,
              and transaction reporting. This project highlighted my ability to integrate a dynamic
              user interface with secure and scalable API services.
            </p>
          </div>

          <div class="flex justify-between mt-6">
            <ul class="flex gap-3">
              <li class="icon-box"><Icon icon="simple-icons:express" /></li>
              <li class="icon-box"><Icon icon="logos:react" /></li>
              <li class="icon-box"><Icon icon="logos:tailwindcss-icon" /></li>
              <li class="icon-box"><Icon icon="logos:nodejs-icon" /></li>
            </ul>
            <button class="btn-clean">Github</button>
          </div>
        </div>
      </div>

      <!-- ================= CARD 5 ================= -->
      <div class="card-clean grid md:grid-cols-2 gap-10 items-center p-8 rounded-2xl">
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-semibold">CukurRans</h2>
            <p class="text-gray-400 font-dmSans">
              Cukurans: Digital Barbershop Booking & Management System Cukurans is a digital
              solution designed to modernize conventional barbershop services. This platform allows
              users to book appointments online while also helping barbershop owners manage queues
              and barber schedules efficiently. With a decoupled architecture, the system ensures
              fast performance on the user side and secure data management on the server side.
            </p>
          </div>

          <div class="flex justify-between mt-6">
            <ul class="flex gap-3">
              <li class="icon-box"><Icon icon="simple-icons:express" /></li>
              <li class="icon-box"><Icon icon="logos:react" /></li>
              <li class="icon-box"><Icon icon="logos:tailwindcss-icon" /></li>
              <li class="icon-box"><Icon icon="logos:nodejs-icon" /></li>
            </ul>
            <button class="btn-clean">Github</button>
          </div>
        </div>

        <div class="image-box">
          <img src="./icons/Cukur.png" />
        </div>
      </div>
    </div>
    <!-- CURVED ARROW -->
    <div class="mt-8 flex justify-center md:justify-end left-0">
      <svg class="w-20 h-20 text-purple-400 animate-fadeIn" viewBox="0 0 100 100" fill="none">
        <!-- path melengkung -->
        <path
          d="M20 20 C20 60, 80 40, 80 80"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          class="animate-draw"
        />

        <!-- arrow head -->
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
.card-clean {
  position: relative;
  background: rgba(24, 24, 27, 0.85);
  backdrop-filter: blur(12px);
  border-radius: 1rem;
  overflow: hidden;
}

/* BORDER */
.card-clean::before {
  content: '';
  position: absolute;
  inset: 0;
  padding: 1px;
  border-radius: inherit;

  background: linear-gradient(
    120deg,
    rgba(0, 255, 255, 0.25),
    rgba(139, 92, 246, 0.25),
    rgba(236, 72, 153, 0.25)
  );

  -webkit-mask:
    linear-gradient(#fff 0 0) content-box,
    linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
  mask-composite: exclude;
}

/* GLOW */
.card-clean::after {
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

  filter: blur(10px);
  opacity: 0.4;
  z-index: -1;
}

/* IMAGE */
.image-box {
  position: relative;
  height: 280px;
  overflow: hidden;
  border-radius: 0.75rem;
}

.image-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: 0.5s;
}

.image-box img:hover {
  transform: scale(1.05);
}

/* ICON */
.icon-box {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 32px;
  height: 32px;
  background: #27272a;
  border-radius: 6px;
  font-size: 18px;
}

/* BUTTON */
.btn-clean {
  background: white;
  color: black;
  font-size: 12px;
  padding: 6px 14px;
  border-radius: 6px;
  transition: 0.2s;
}

.btn-clean:hover {
  opacity: 0.8;
}
</style>
