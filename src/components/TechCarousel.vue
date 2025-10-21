<template>
  <div class="carousel-container">
    <div class="carousel-track">
      <div class="carousel-content">
        <img
          v-for="(logo, index) in logos"
          :key="`logo-${index}`"
          :src="logo.src"
          :alt="logo.alt"
          class="tech-logo"
        />
      </div>
      <div class="carousel-content" aria-hidden="true">
        <img
          v-for="(logo, index) in logos"
          :key="`logo-duplicate-${index}`"
          :src="logo.src"
          :alt="logo.alt"
          class="tech-logo"
        />
      </div>
    </div>
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
.carousel-container {
  width: 100%;
  overflow: hidden;
  padding: 40px 0;
  position: relative;
}

.carousel-track {
  display: flex;
  width: fit-content;
  animation: scroll 30s linear infinite;
}

.carousel-content {
  display: flex;
  gap: 80px;
  align-items: center;
  padding: 0 40px;
}

.tech-logo {
  height: 60px;
  width: auto;
  object-fit: contain;
  filter: grayscale(100%) opacity(0.6);
  transition: filter 0.3s ease;
}

.tech-logo:hover {
  filter: grayscale(0%) opacity(1);
}

@keyframes scroll {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-50%);
  }
}

/* Pause animation on hover */
.carousel-track:hover {
  animation-play-state: paused;
}

@media (max-width: 768px) {
  .carousel-content {
    gap: 50px;
    padding: 0 20px;
  }

  .tech-logo {
    height: 45px;
  }
}
</style>
