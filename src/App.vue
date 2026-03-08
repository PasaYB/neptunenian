<script setup>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import CatalogueSection from './components/CatalogueSection.vue'
import AboutSection from './components/AboutSection.vue'
import ReviewSection from './components/ReviewSection.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <div class="bg-white dark:bg-black transition-colors duration-300">
    <NavBar />
    <HeroSection />
    <AboutSection />
    <CatalogueSection />
    <ReviewSection />
    <AppFooter />
  </div>
</template>
