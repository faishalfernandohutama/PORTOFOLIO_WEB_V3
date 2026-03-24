<template>
  <section
    class="min-h-screen flex flex-col justify-center text-white px-6 max-w-7xl mx-auto relative z-10"
  >
    <div class="font-dmSans mb-16 space-y-4 text-center md:text-left">
      <p class="text-purple-400 uppercase tracking-widest text-sm font-semibold">Contact</p>
      <h1
        class="text-4xl md:text-5xl lg:text-6xl font-changaOne uppercase tracking-wide leading-tight"
      >
        Ready to cut the noise and <span class="text-purple-400">execute?</span>
      </h1>
    </div>

    <div class="grid md:grid-cols-2 gap-12 lg:gap-20 items-start border-t border-white/10 pt-12">
      <div class="space-y-8 text-center md:text-left">
        <div class="space-y-4">
          <h2 class="text-3xl font-changaOne uppercase tracking-wide">How can I help?</h2>
          <p class="font-dmSans text-white/70 leading-relaxed max-w-md mx-auto md:mx-0">
            I would love to hear more about your project. Whether you need a high-performance web
            solution, system management, or just want to discuss strategy, let's make it happen.
          </p>
        </div>

        <div class="space-y-2 font-dmSans text-white/80">
          <a
            href="mailto:nandolop71@gmail.com"
            class="block text-lg hover:text-purple-400 transition-colors duration-300"
          >
            nandolop71@gmail.com
          </a>
          <p class="text-white/50 text-sm">Sidoarjo, East Java, Indonesia</p>
        </div>
      </div>

      <div class="bg-white/5 border border-white/10 rounded-2xl p-6 md:p-8 backdrop-blur-xl">
        <form class="space-y-6 font-dmSans" @submit.prevent>
          <div class="grid grid-cols-2 gap-4">
            <div class="col-span-2 md:col-span-1">
              <label class="block text-sm text-white/60 mb-2">Name</label>
              <input
                type="text"
                class="w-full bg-black/50 border border-white/10 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-purple-500 transition-colors"
                placeholder="Your name"
              />
            </div>
            <div class="col-span-2 md:col-span-1">
              <label class="block text-sm text-white/60 mb-2">Email</label>
              <input
                type="email"
                class="w-full bg-black/50 border border-white/10 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-purple-500 transition-colors"
                placeholder="you@example.com"
              />
            </div>
          </div>

          <div>
            <label class="block text-sm text-white/60 mb-2">Message</label>
            <textarea
              rows="4"
              class="w-full bg-black/50 border border-white/10 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-purple-500 transition-colors resize-none"
              placeholder="Tell me about your project..."
            ></textarea>
          </div>

          <button
            type="submit"
            class="w-full bg-white text-black font-semibold py-3.5 rounded-lg hover:bg-purple-500 hover:text-white transition-all duration-300 uppercase tracking-wider text-sm"
          >
            Send Message
          </button>
        </form>
      </div>
    </div>
  </section>
</template>
