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
}

main {
  width: 100%;
}
</style>
