<template>
  <section class="relative w-full h-screen min-h-[600px] flex flex-col justify-end">
    <!-- Background image -->

    <!-- Cloud assets desktop -->
    <div class="hidden lg:block">
      <img class="absolute size-[25%] top-[3rem] left-[9%] z-20" src="/public/img/cloud.png" alt="c">
      <img class="absolute size-[25%] top-[30rem] left-[26%] z-20" src="/public/img/cloud.png" alt="c">
      <img class="absolute size-[25%] top-[9rem] left-[76%] z-20" src="/public/img/cloud.png" alt="c">
      <img class="absolute size-[25%] top-[32rem] left-[66%] z-20" src="/public/img/cloud.png" alt="c">
    </div>

    <img class="absolute w-full top-[2rem] left-[28%] z-20 lg:hidden dark:opacity-60" src="/public/img/cloud.png" alt="c">
    <img class="absolute w-full top-[25rem] right-[24%] z-20 lg:hidden dark:opacity-50" src="/public/img/cloud.png" alt="c">
    

    <!-- mobile -->
    <div class="absolute lg:hidden inset-0 bg-gradient-to-b from-cyan-400 to-neutral-50 dark:from-cyan-700 dark:to-black rounded-br-3xl rounded-bl-3xl shadow-[0_10px_12px_1px_rgba(0,0,0,0.1)]">
    </div>


    <!-- desktop -->
    <div class="absolute hidden lg:block inset-20 rounded-3xl bg-gradient-to-b from-cyan-400 to-neutral-50 dark:to-black">
      <!-- <img src="/img/hero.png" alt="" class="w-full h-full object-cover" /> -->
      <div class="flex flex-col justify-between h-full">
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 p-10">
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 p-10">
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
          <p class="text-yellow-400 font-semibold text-center text-shadow-lg/50">Neptunenian</p>
        </div>
        </div>
    </div>

    <!-- Overlay -->
    <!-- <div class="absolute inset-0"></div> -->

    <!-- Content -->
    <div class="relative z-10 px-6 sm:px-8 pb-[20rem] sm:pb-[16rem] max-w-3xl">
      <!-- <h1 class="text-5xl sm:text-7xl md:text-8xl font-bold text-white leading-none mb-4">
        Neptunenian
      </h1> -->
      <!-- <p class="text-white/80 text-sm sm:text-base max-w-sm leading-relaxed">
        Hi there, welcome to neptoon's page. Looking for a design that suit your preferences? Explore at our designs project! Contact us for more details
      </p> -->
    </div>
  </section>
</template>