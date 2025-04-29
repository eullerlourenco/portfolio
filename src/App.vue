<template>
  <div class="min-h-screen">
    <Header />
    <main>
      <Hero />
      <About />
      <Projects />
      <div class="container mx-auto px-4 py-50">
        more content here

      </div>
    </main>
  <Footer />
  </div>
</template>

<script setup>

import Header from './components/Header.vue';
import About from './components/sections/About.vue';
import Hero from './components/sections/Hero.vue';
import Projects from './components/sections/Projects.vue';
import Footer from './components/sections/Footer.vue';

</script>
