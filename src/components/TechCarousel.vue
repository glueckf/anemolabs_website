<template>
  <div class="tech-logos-container">
    <img
      v-for="(logo, index) in logos"
      :key="`logo-${index}`"
      :src="logo.src"
      :alt="logo.alt"
      class="tech-logo"
    />
  </div>
</template>

<script setup>
import pythonLogo from '../assets/Software Icons/black_for_light_background/python-logo-only 1.png'
import fastapiLogo from '../assets/Software Icons/black_for_light_background/FastAPI.png'
import dockerLogo from '../assets/Software Icons/black_for_light_background/docker-mark-blue-2.png'
import typescriptLogo from '../assets/Software Icons/black_for_light_background/ts-logo-256.png'
import vueLogo from '../assets/Software Icons/black_for_light_background/vue.png'

const logos = [
  { src: pythonLogo, alt: 'Python' },
  { src: fastapiLogo, alt: 'FastAPI' },
  { src: dockerLogo, alt: 'Docker' },
  { src: typescriptLogo, alt: 'TypeScript' },
  { src: vueLogo, alt: 'Vue.js' }
]
</script>

<style scoped>
.tech-logos-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  padding: 40px 0;
}

.tech-logo {
  height: 50px;
  width: auto;
  object-fit: contain;
  filter: grayscale(100%);
  opacity: 0.7;
}

@media (max-width: 768px) {
  .tech-logos-container {
    gap: 20px;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  .tech-logo {
    height: 40px;
  }
}
</style>
