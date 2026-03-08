<template>
  <section class="py-16 pb-8 px-4 sm:px-6 bg-white dark:bg-black" id="about">
    <div class="max-w-[72rem] mx-auto">
      <!-- Badge row -->
      <div class="flex flex-col sm:flex-row sm:items-center justify-between mb-10 gap-4">
        <div class="flex flex-wrap items-center gap-4 sm:gap-6 text-sm text-black dark:text-white">
          <span class="flex items-center gap-2">
            <span class="text-base">🎨</span> We are Neptunenian
          </span>
          <span class="flex items-center gap-2">
            <span class="text-base">⭐</span> 100+ Satisfied Clients
          </span>
        </div>
      </div>

      <!-- Heading -->
      <h2 class="text-4xl sm:text-5xl md:text-6xl font-bold text-black dark:text-white leading-tight mb-4">
        Neptunenian means<br />Quality 
      </h2>

      <p class="text-sm sm:text-base text-black dark:text-gray-400 max-w-xl leading-relaxed mb-6">
        Hi there, welcome to neptoon's page. Looking for a design that suit your preferences? Explore at our designs project! Contact us for more details
      </p>

      <button class="bg-[#00d757] rounded-full p-4 dark:text-white shadow-lg">
        <i class="fa fa-whatsapp" style="font-size: 20px;"></i> Whatsapp
      </button>

      <!-- Dotted line accent -->
      <div class="flex items-center gap-0.5 mt-8">
        <div class="flex-1 border-t-2 border-dashed border-black dark:border-white"></div>
        <div class="w-5 h-5 rounded-full border-2 border-yellow-500 flex items-center justify-center">
          <div class="w-2 h-2 rounded-full bg-yellow-500"></div>
        </div>
      </div>
    </div>
  </section>
</template>


<style scoped>
button {
  transition: 0.5s; 
  animation: gradient_301 5s ease infinite;
}

button:hover {
  transform: scale(1.05);
}
</style>