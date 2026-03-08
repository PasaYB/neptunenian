<script setup>
const items = [
  { name: 'Custom Banner', category: 'Banner', size: '60×160 cm', price: 'Rp 20.000', tag: 'Best Seller', image: '/img/catalogue/banner/banner1.png' },
  { name: 'Pop Mart: Crying For A Degree', category: 'Banner', size: '200×100 cm', price: 'Rp 20.000', tag: null, image: '/img/catalogue/banner/banner2.png' },
{ name: 'Totally Spies: Totally Grads', category: 'Banner', size: '60×160 cm', price: 'Rp 20.000', tag: 'Popular', image: '/img/catalogue/banner/banner3.png' },
{ name: 'Kartu Sidang', category: 'Banner', size: '85×200 cm', price: 'Rp 200.000', tag: null, image: '/img/catalogue/banner/banner4.png' },
{ name: 'Struk Sidang', category: 'Banner', size: 'Custom Size', price: 'Rp 20.000', tag: null, image: '/img/catalogue/banner/banner5.png' },
{ name: 'How We Met Our Degree', category: 'Banner', size: '3×2 m', price: 'Rp 200.000', tag: 'New', image: '/img/catalogue/banner/banner6.png' },
]
</script>

<template>
  <section class="py-16 px-4 sm:px-6 bg-white dark:bg-black" id="catalogue">
    <div class="max-w-6xl mx-auto">
      <!-- Header -->
      <div class="flex flex-col md:flex-row md:items-end justify-between mb-10 gap-4">
        <div>
          <p class="text-xs text-gray-400 mb-2 flex items-center gap-1">
            <span class="w-1.5 h-1.5 rounded-full bg-yellow-400 inline-block"></span>
            Our Products
          </p>
          <h2 class="text-4xl sm:text-5xl font-bold text-gray-900 dark:text-white">Our Catalogue</h2>
        </div>
        <p class="text-sm text-gray-500 dark:text-gray-400 md:max-w-xs md:text-right">
          High quality custom design, ready to order.
        </p>
      </div>

      <!-- Filter row -->
       <!-- TODO: Filter button -->
      <div class="flex flex-wrap items-end gap-4 mb-8">
        <div class="flex-1 min-w-32">
          <p class="text-sm text-gray-400 mb-1">Category</p>
          <p class="text-xs text-gray-400 mb-1">All</p>
        </div>
      </div>

      <!-- Cards grid -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
        <div
          v-for="item in items"
          :key="item.name"
          class="rounded-2xl overflow-hidden border border-gray-100 dark:border-[#3E3E3E] shadow-sm
                 bg-white dark:bg-[#2E2E2E] hover:shadow-md transition-shadow dark:shadow-[0_4px_8px_0_rgba(255,255,255,0.3)]"
        >
          <!-- Image -->
          <div class="relative h-48 bg-gray-100 dark:bg-[#2E2E2E] overflow-hidden">
            <img
              :src="item.image"
              :alt="item.name"
              class="w-full h-[132%] object-cover object-center transition-transform duration-500 hover:scale-105"
            />
            <div class="absolute inset-0 bg-gradient-to-t from-black/30 to-transparent"></div>
            <span
              v-if="item.tag"
              class="absolute top-3 left-3 text-xs bg-gray-900 dark:bg-white text-white dark:text-gray-900
                     px-2 py-0.5 rounded-full font-semibold"
            >
              {{ item.tag }}
            </span>
          </div>

          <!-- Card body -->
          <div class="p-4">
            <div class="flex items-start justify-between mb-1">
              <h3 class="font-semibold text-gray-900 dark:text-white text-sm">{{ item.name }}</h3>
              <span class="text-xs text-gray-400 dark:text-white bg-gray-100 dark:bg-[#4E4E4E] px-2 py-0.5 rounded-full mb-3">
                {{ item.category }}
              </span>
            </div>
            <!-- <p class="text-xs text-gray-400 mb-3">{{ item.size }}</p> -->
            <div class="flex items-center justify-between border-t border-gray-100 dark:border-[#4E4E4E] pt-3">
              <span class="text-sm font-bold text-gray-900 dark:text-white">{{ item.price }}</span>
              <!-- <button class="text-xs px-3 py-1.5 bg-gray-900 dark:bg-white text-white dark:text-gray-900
                             rounded-full font-semibold hover:opacity-80 transition-opacity">
                Order
              </button> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
