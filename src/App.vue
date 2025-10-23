<template>
  <div id="app">
    <TheHeader />
    <main>
      <LandingSection />
      <WhatWeDoSection />
      <AboutUsSection />
      <ProjectsSection />
      <ContactSection />
    </main>
    <TheFooter />
  </div>
</template>

<script setup>
import TheHeader from './components/TheHeader.vue'
import LandingSection from './components/LandingSection.vue'
import WhatWeDoSection from './components/WhatWeDoSection.vue'
import AboutUsSection from './components/AboutUsSection.vue'
import ProjectsSection from './components/ProjectsSection.vue'
import ContactSection from './components/ContactSection.vue'
import TheFooter from './components/TheFooter.vue'
</script>

<style>
#app {
  width: 100%;
  min-height: 100vh;
  background-color: #f5f5f5;
}

main {
  width: 100%;
  max-width: 1400px;
  margin: 0 auto;
  padding: 40px 80px;
}

@media (max-width: 768px) {
  main {
    padding: 20px;
  }
}
</style>
