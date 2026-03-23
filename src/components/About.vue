<template>
  <section
    class="grid gap-12 md:grid-cols-2 items-center text-white px-6 pt-20 pb-8 max-w-7xl mx-auto"
  >
    <div class="space-y-6 max-w-lg">
      <h1 class="text-3xl md:text-4xl font-changaOne uppercase tracking-wide leading-tight">
        About Me
      </h1>

      <p class="text-sm md:text-base text-white/70 leading-relaxed">
        I’m a developer with a strong interest in modern web design and clean user experiences. I
        enjoy turning ideas into interactive and functional digital products.
      </p>

      <div class="w-16 h-[2px] bg-gradient-to-r from-purple-500 to-transparent"></div>

      <ul class="space-y-3 text-sm md:text-base text-white/80">
        <li class="flex items-start gap-3">
          <span class="text-purple-400 mt-1">•</span>
          Building modern and responsive websites
        </li>
        <li class="flex items-start gap-3">
          <span class="text-purple-400 mt-1">•</span>
          Managing and maintaining data systems
        </li>
        <li class="flex items-start gap-3">
          <span class="text-purple-400 mt-1">•</span>
          Delivering solutions based on client needs
        </li>
      </ul>

      <div class="flex justify-center md:justify-start pt-4">
        <svg class="w-16 h-16 text-purple-400 animate-fadeIn" viewBox="0 0 100 100" fill="none">
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
    </div>

    <div class="relative grid gap-6">
      <div class="relative group rounded-2xl">
        <div
          class="absolute -inset-[1px] rounded-2xl bg-[linear-gradient(120deg,#a855f7,#6366f1,#a855f7)] bg-[length:200%_100%] animate-gradient opacity-80 blur-md group-hover:opacity-100 transition duration-300"
        ></div>
        <div class="relative bg-black/60 border border-white/10 rounded-2xl p-6 backdrop-blur-xl">
          <h2 class="text-lg md:text-xl font-changaOne uppercase mb-2">Web Development</h2>
          <p class="text-sm text-white/70 leading-relaxed">
            Building modern, responsive, and high-performance websites with a focus on clean
            architecture and scalability.
          </p>
        </div>
      </div>

      <div class="relative group rounded-2xl">
        <div
          class="absolute -inset-[1px] rounded-2xl bg-[linear-gradient(120deg,#a855f7,#6366f1,#a855f7)] bg-[length:200%_100%] animate-gradient opacity-80 blur-md group-hover:opacity-100 transition duration-300"
        ></div>
        <div class="relative bg-black/60 border border-white/10 rounded-2xl p-6 backdrop-blur-xl">
          <h2 class="text-lg md:text-xl font-changaOne uppercase">UI / UX Design</h2>
          <p class="text-sm text-white/70 leading-relaxed">
            Designing intuitive and visually engaging user interfaces that enhance usability and
            create meaningful user experiences.
          </p>
        </div>
      </div>

      <div class="relative group rounded-2xl">
        <div
          class="absolute -inset-[1px] rounded-2xl bg-[linear-gradient(120deg,#a855f7,#6366f1,#a855f7)] bg-[length:200%_100%] animate-gradient opacity-80 blur-md group-hover:opacity-100 transition duration-300"
        ></div>
        <div class="relative bg-black/60 border border-white/10 rounded-2xl p-6 backdrop-blur-xl">
          <h2 class="text-lg md:text-xl font-changaOne uppercase">Data & System Management</h2>
          <p class="text-sm text-white/70 leading-relaxed">
            Managing structured data and maintaining systems to ensure efficiency, reliability, and
            long-term sustainability.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
@keyframes gradientMove {
  0% {
    background-position: 0% 50%;
  }
  100% {
    background-position: 200% 50%;
  }
}

.animate-gradient {
  animation: gradientMove 3s linear infinite;
}

/* fade masuk */
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

/* efek garis digambar */
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

/* arrow bounce */
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
