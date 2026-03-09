<template>
  <footer class="bg-gray-30 shadow-[0_-10px_12px_2px_rgba(0,0,0,0.1)] dark:shadow-[0_-10px_12px_2px_rgba(255,255,255,0.1)] dark:bg-black rounded-tr-3xl rounded-tl-3xl border-t dark:border-[#4E4E4E]">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 py-12">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 mb-10">
        <div class="flex items-center">
          <span class="font-bold text-black text-xl dark:text-white">Neptunenian</span>
        </div>
        
        <!-- Products -->
        <div>
          <h4 class="text-sm font-semibold text-black dark:text-white mb-3">Products</h4>
          <ul class="space-y-2 text-sm text-gray-500 dark:text-gray-400">
            <li><a class="hover:text-yellow-400 transition-colors">Vertical Banner</a></li>
            <li><a class="hover:text-yellow-400 transition-colors">X-Banner</a></li>
            <li><a class="hover:text-yellow-400 transition-colors">Roll Up Banner</a></li>
            <li><a class="hover:text-yellow-400 transition-colors">Backdrop</a></li>
          </ul>
        </div>

        <!-- Company -->
        <div>
          <h4 class="text-sm font-semibold text-black dark:text-white mb-3">Company</h4>
          <ul class="space-y-2 text-sm text-gray-500 dark:text-gray-400">
            <li><a class="hover:text-yellow-400 transition-colors">About Us</a></li>
            <li><a class="hover:text-yellow-400 transition-colors">Pricing</a></li>
            <li><a class="hover:text-yellow-400 transition-colors">Reviews</a></li>
            <li><a class="hover:text-yellow-400 transition-colors">Contact</a></li>
          </ul>
        </div>

        <!-- Contact -->
        <div>
          <h4 class="text-sm font-semibold text-black dark:text-white mb-3">Get in Touch</h4>
          <ul class="flex space-x-3 text-sm text-gray-500 dark:text-gray-400">
            <li><i class="fa fa-whatsapp" style="font-size:16px"></i></li>
            <li><i class="fa fa-twitter"></i> </li>
            <li><i class="fa fa-instagram"></i> </li>
          </ul>
        </div>
      </div>

      <!-- Bottom bar -->
      <div class="border-t border-black dark:border-[#4E4E4E] pt-6 flex flex-col sm:flex-row items-center justify-between gap-2 text-xs text-black dark:text-gray-400">
        <span>© 2025 Neptunenian. All rights reserved.</span>
      </div>
    </div>
  </footer>
</template>
