<script setup>
const reviews = [
  {
    initials: 'DJ',
    name: 'Donald Jackman',
    rating: 5,
    color: 'bg-red-500',
    text: "The banner turned out amazing! Great quality print and delivered right on time. Highly recommended for any event.",
  },
  {
    initials: 'SA',
    name: 'Siti Aminah',
    rating: 5,
    color: 'bg-blue-500',
    text: "Sudah pesan beberapa kali dan hasilnya selalu memuaskan. Warna tajam, bahan kuat, harga terjangkau.",
  },
  {
    initials: 'RH',
    name: 'Ryan Hendra',
    rating: 5,
    color: 'bg-green-500',
    text: "Fast response, fast production. The roll up banner looks super professional. Will order again for our next booth!",
  },
  {
    initials: 'NF',
    name: 'Nadia Fitri',
    rating: 5,
    color: 'bg-purple-500',
    text: "Backdrop-nya keren banget buat acara wedding. Responsif, proses cepat, dan hasilnya melebihi ekspektasi.",
  },
  {
    initials: 'BP',
    name: 'Budi Pratama',
    rating: 4,
    color: 'bg-orange-500',
    text: "Good quality banner at a very competitive price. The x-banner holds up well outdoors. Very happy with the result.",
  },
  {
    initials: 'LD',
    name: 'Luna Dewi',
    rating: 5,
    color: 'bg-pink-500',
    text: "Pelayanan ramah dan profesional. Desain dibantuin juga! Hasilnya persis sesuai keinginan saya.",
  },
]
</script>

<template>
  <section class="py-16 pb-36 bg-white dark:bg-black overflow-hidden" id="review">
    <!-- Section header -->
    <div class="px-4 sm:px-6 mb-10 max-w-6xl mx-auto">
      <p class="text-xs text-gray-500 dark:text-gray-400 mb-2 flex items-center gap-1">
        <span class="w-1.5 h-1.5 rounded-full bg-yellow-400 inline-block"></span>
        Testimonials
      </p>
      <h2 class="text-4xl sm:text-5xl font-bold text-black dark:text-white">What They Say</h2>
    </div>

    <!-- Marquee track -->
    <div class="relative">
      <!-- Fade edges -->
      <div class="pointer-events-none absolute left-0 top-0 bottom-0 w-24 z-10
                  bg-gradient-to-r from-white dark:from-black to-transparent"></div>
      <div class="pointer-events-none absolute right-0 top-0 bottom-0 w-24 z-10
                  bg-gradient-to-l from-white dark:from-black to-transparent"></div>

      <div class="marquee-wrapper flex gap-5 w-max">
        <!-- Render items twice for seamless loop -->
        <div
          v-for="(review, i) in [...reviews, ...reviews]"
          :key="i"
          class="w-72 shrink-0 rounded-2xl border border-gray-200 dark:border-[#4E4E4E]
                 bg-white dark:bg-[#2E2E2E] shadow-lg dark:shadow-[0_4px_8px_0_rgba(255,255,255,0.3)] p-6 space-y-4"
        >
          <!-- Avatar + name -->
          <div class="flex items-center gap-3">
            <div :class="[review.color, 'h-11 w-11 flex items-center justify-center text-white text-sm font-bold rounded-full shrink-0']">
              {{ review.initials }}
            </div>
            <span class="text-sm font-medium text-black dark:text-white">{{ review.name }}</span>
          </div>

          <!-- Stars -->
          <div class="flex gap-0.5">
            <span
              v-for="n in 5"
              :key="n"
              :class="n <= review.rating ? 'text-yellow-400' : 'text-gray-300 dark:text-gray-600'"
              class="text-lg leading-none"
            >★</span>
          </div>

          <!-- Review text -->
          <p class="text-sm text-gray-700 dark:text-gray-300 leading-relaxed">
            {{ review.text }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.marquee-wrapper {
  animation: marquee 35s linear infinite;
}

.marquee-wrapper:hover {
  animation-play-state: paused;
}

@keyframes marquee {
  0%   { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}
</style>
