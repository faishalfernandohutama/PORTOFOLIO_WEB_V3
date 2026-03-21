<template>
  <section class="grid gap-16 text-white px-6 max-w-7xl mx-auto">
    <!-- TITLE -->
    <div class="text-center">
      <h1 class="text-3xl md:text-4xl lg:text-6xl font-changaOne">EVERYTHING ABOUT MY PROJECT</h1>
    </div>

    <!-- CARD LIST -->
    <div class="grid gap-12">
      <!-- ================= CARD 1 ================= -->
      <div class="grid md:grid-cols-2 gap-10 items-center bg-zinc-900 p-8 rounded-2xl">
        <!-- TEXT -->
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-changaOne">CLUPPER CRAFTERS</h2>
            <p class="text-gray-400 leading-relaxed">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>

          <div class="flex items-center justify-between mt-6">
            <ul class="flex gap-2 text-xs">
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Vue</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Tailwind</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">API</li>
            </ul>

            <button
              class="bg-white text-black text-xs px-4 py-2 rounded-md hover:opacity-80 transition"
            >
              Github
            </button>
          </div>
        </div>

        <!-- IMAGE -->
        <div class="relative rounded-xl overflow-hidden h-[280px]">
          <!-- BASE BACKGROUND -->
          <div class="absolute inset-0 bg-[#0A0F3C]"></div>

          <!-- RADIAL GLOW -->
          <div
            class="absolute inset-0 bg-[radial-gradient(circle_at_70%_50%,_#C84DFF_0%,_#7B1FA2_25%,_#3B0F70_50%,_transparent_75%)]"
          ></div>

          <!-- IMAGE -->
          <img
            src="./icons/clip.png"
            alt="Clupper Crafters Preview"
            class="relative w-full h-full object-cover transition duration-500 hover:scale-105"
          />
        </div>
      </div>

      <!-- ================= CARD 2 ================= -->
      <div class="grid md:grid-cols-2 gap-10 items-center bg-zinc-900 p-8 rounded-2xl">
        <!-- IMAGE -->
        <div class="relative rounded-xl overflow-hidden h-[280px] order-1 md:order-none">
          <!-- BASE BACKGROUND -->
          <div class="absolute inset-0 bg-[#0A0F3C]"></div>

          <!-- RADIAL GLOW (reverse direction) -->
          <div
            class="absolute inset-0 bg-[radial-gradient(circle_at_30%_50%,_#C84DFF_0%,_#7B1FA2_25%,_#3B0F70_50%,_transparent_75%)]"
          ></div>

          <!-- IMAGE -->
          <img
            src="./icons/ERP.png"
            alt="Project 2 Preview"
            class="relative w-full h-full object-cover transition duration-500 hover:scale-105"
          />
        </div>

        <!-- TEXT -->
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-changaOne">ERP Project</h2>
            <p class="text-gray-400 leading-relaxed">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>

          <div class="flex items-center justify-between mt-6">
            <ul class="flex gap-2 text-xs">
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Vue</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Tailwind</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">API</li>
            </ul>

            <button
              class="bg-white text-black text-xs px-4 py-2 rounded-md hover:opacity-80 transition"
            >
              Github
            </button>
          </div>
        </div>
      </div>

      <!-- ================= CARD 3 ================= -->
      <div class="grid md:grid-cols-2 gap-10 items-center bg-zinc-900 p-8 rounded-2xl">
        <!-- TEXT -->
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-changaOne">CatBoost Prediction</h2>
            <p class="text-gray-400 leading-relaxed">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>

          <div class="flex items-center justify-between mt-6">
            <ul class="flex gap-2 text-xs">
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Vue</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Tailwind</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">API</li>
            </ul>

            <button
              class="bg-white text-black text-xs px-4 py-2 rounded-md hover:opacity-80 transition"
            >
              Github
            </button>
          </div>
        </div>

        <!-- IMAGE -->
        <div class="relative rounded-xl overflow-hidden h-[280px]">
          <!-- BASE BACKGROUND -->
          <div class="absolute inset-0 bg-[#0A0F3C]"></div>

          <!-- RADIAL GLOW -->
          <div
            class="absolute inset-0 bg-[radial-gradient(circle_at_70%_50%,_#C84DFF_0%,_#7B1FA2_25%,_#3B0F70_50%,_transparent_75%)]"
          ></div>

          <!-- IMAGE -->
          <img
            src="./icons/cat.png"
            alt="Clupper Crafters Preview"
            class="relative w-full h-full object-cover transition duration-500 hover:scale-105"
          />
        </div>
      </div>
      <!-- ================= CARD 4 ================= -->
      <div class="grid md:grid-cols-2 gap-10 items-center bg-zinc-900 p-8 rounded-2xl">
        <!-- IMAGE -->
        <div class="relative rounded-xl overflow-hidden h-[280px] order-1 md:order-none">
          <!-- BASE BACKGROUND -->
          <div class="absolute inset-0 bg-[#0A0F3C]"></div>

          <!-- RADIAL GLOW (reverse direction) -->
          <div
            class="absolute inset-0 bg-[radial-gradient(circle_at_30%_50%,_#C84DFF_0%,_#7B1FA2_25%,_#3B0F70_50%,_transparent_75%)]"
          ></div>

          <!-- IMAGE -->
          <img
            src="./icons/InnHubb.png"
            alt="Project 2 Preview"
            class="relative w-full h-full object-cover transition duration-500 hover:scale-105"
          />
        </div>

        <!-- TEXT -->
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-changaOne">InnHub</h2>
            <p class="text-gray-400 leading-relaxed">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>

          <div class="flex items-center justify-between mt-6">
            <ul class="flex gap-2 text-xs">
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Vue</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Tailwind</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">API</li>
            </ul>

            <button
              class="bg-white text-black text-xs px-4 py-2 rounded-md hover:opacity-80 transition"
            >
              Github
            </button>
          </div>
        </div>
      </div>
      <!-- ================= CARD 5 ================= -->
      <div class="grid md:grid-cols-2 gap-10 items-center bg-zinc-900 p-8 rounded-2xl">
        <!-- TEXT -->
        <div class="flex flex-col justify-between h-full">
          <div class="space-y-4">
            <h2 class="uppercase text-2xl font-changaOne">CukurRans</h2>
            <p class="text-gray-400 leading-relaxed">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
          </div>

          <div class="flex items-center justify-between mt-6">
            <ul class="flex gap-2 text-xs">
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Vue</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">Tailwind</li>
              <li class="bg-zinc-800 px-3 py-1 rounded-full">API</li>
            </ul>

            <button
              class="bg-white text-black text-xs px-4 py-2 rounded-md hover:opacity-80 transition"
            >
              Github
            </button>
          </div>
        </div>

        <!-- IMAGE -->
        <div class="relative rounded-xl overflow-hidden h-[280px]">
          <!-- BASE BACKGROUND -->
          <div class="absolute inset-0 bg-[#0A0F3C]"></div>

          <!-- RADIAL GLOW -->
          <div
            class="absolute inset-0 bg-[radial-gradient(circle_at_70%_50%,_#C84DFF_0%,_#7B1FA2_25%,_#3B0F70_50%,_transparent_75%)]"
          ></div>

          <!-- IMAGE -->
          <img
            src="./icons/Cukur.png"
            alt="Clupper Crafters Preview"
            class="relative w-full h-full object-cover transition duration-500 hover:scale-105"
          />
        </div>
      </div>
    </div>
  </section>
</template>
