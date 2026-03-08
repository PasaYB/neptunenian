<script setup>
import { ref } from 'vue'
import ThemeToggle from './ThemeToggle.vue'

const menuOpen = ref(false)
</script>

<template>
  <nav class="fixed top-0 left-0 right-0 z-50 bg-white/30 dark:bg-black/80 backdrop-blur">
    <div class="flex items-center justify-between px-4 sm:px-6 py-3">
      <!-- Logo -->
      <div class="flex items-center gap-2 shrink-0">
        <div class="w-8 h-8 rounded-full overflow-hidden">
          <img class="rounded-full w-full h-full object-cover" src="/img/profile.png" alt="profile pic" />
        </div>
        <span class="font-semibold text-sm tracking-tight dark:text-white">Neptunenian</span>
      </div>

      <!-- Desktop nav links -->
      <div class="hidden lg:flex items-center gap-6 text-sm text-black dark:text-gray-400">
        <a href="#about" class="hover:text-yellow-600 transition-colors">About us</a>
        <a href="#catalogue" class="hover:text-yellow-600 transition-colors">Catalogue</a>
        <a href="#review" class="hover:text-yellow-600 transition-colors">Reviews</a>
        <a href="#" class="text-green-500 transition-colors">Order Now!</a>
      </div>

      <div class="flex items-center gap-2">
        <ThemeToggle />
        <!-- Hamburger (mobile) -->
        <button
          class="lg:hidden p-1.5 rounded-md text-gray-600 dark:text-gray-400
                 transition-colors"
          @click="menuOpen = !menuOpen"
          aria-label="Toggle menu"
        >
          <svg v-if="!menuOpen" class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16"/>
          </svg>
          <svg v-else class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/>
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile dropdown menu -->
    <div
      v-if="menuOpen"
      class="lg:hidden dark:border-gray-700 bg-white/40 dark:bg-black/40 backdrop-blur-none"
    >
      <div class="flex flex-col px-4 py-3 gap-1">
        <a href="#about" class="py-2 px-3 text-sm rounded-lg text-gray-700 dark:text-gray-300
                           hover:bg-gray-100 dark:hover:bg-gray-800 transition-colors"
           @click="menuOpen = false">About us</a>
        <a href="#catalogue" class="py-2 px-3 text-sm rounded-lg text-gray-700 dark:text-gray-300
                           hover:bg-gray-100 dark:hover:bg-gray-800 transition-colors"
           @click="menuOpen = false">Catalogue</a>
        <a href="#review" class="py-2 px-3 text-sm rounded-lg text-gray-700 dark:text-gray-300
                           hover:bg-gray-100 dark:hover:bg-gray-800 transition-colors"
           @click="menuOpen = false">Reviews</a>3
      </div>
    </div>
  </nav>
</template>
