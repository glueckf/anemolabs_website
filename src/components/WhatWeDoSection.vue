<template>
  <section class="what-we-do">
    <!-- Top Grid: Heading and Description -->
    <div class="top-grid">
      <div class="heading-column">
        <h2 class="main-heading">SOFTWARE THAT FLOWS</h2>
      </div>
      <div class="description-column">
        <p>
          We create custom software solutions designed for performance, scalability and
          maintainability. Every project follows industry best practices with a focus on
          clean architecture.
        </p>
      </div>
    </div>

    <!-- Bottom Section: Our Approach -->
    <div class="approach-section">
      <h3 class="approach-heading">OUR APPROACH</h3>
      <ul class="approach-list">
        <li>
          <span class="number">01</span>
          <span class="text">Modular systems that adapt to your growing needs</span>
        </li>
        <li>
          <span class="number">02</span>
          <span class="text">Modern tech stack: Vue.js, FastAPI, Python, Docker</span>
        </li>
        <li>
          <span class="number">03</span>
          <span class="text">Comprehensive testing and documentation</span>
        </li>
        <li>
          <span class="number">04</span>
          <span class="text">Seamless integrations (APIs, AI tools, legacy systems)</span>
        </li>
        <li>
          <span class="number">05</span>
          <span class="text">Future-proof architecture that scales with your business</span>
        </li>
      </ul>

      <!-- Tech Carousel -->
      <TechCarousel />
    </div>
  </section>
</template>

<script setup>
import TechCarousel from './TechCarousel.vue'
</script>

<style scoped>
.what-we-do {
  background-color: var(--color-light-primary);
}

.top-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 60px;
  margin-bottom: 80px;
}

.main-heading {
  font-size: 4rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  line-height: 1.1;
  letter-spacing: -0.02em;
}

.description-column p {
  font-size: 1.25rem;
  line-height: 1.8;
  color: var(--color-text-primary);
}

.approach-section {
  margin-top: 60px;
}

.approach-heading {
  font-size: 1.5rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  margin-bottom: 30px;
  letter-spacing: 0.05em;
}

.approach-list {
  list-style: none;
  padding: 0;
  margin-bottom: 60px;
}

.approach-list li {
  display: flex;
  align-items: baseline;
  gap: 20px;
  margin-bottom: 20px;
  font-size: 1.1rem;
}

.approach-list .number {
  font-size: 1rem;
  font-weight: 600;
  color: var(--color-accent);
  min-width: 40px;
}

.approach-list .text {
  flex: 1;
  color: var(--color-text-primary);
}

@media (max-width: 768px) {
  .top-grid {
    grid-template-columns: 1fr;
    gap: 30px;
    margin-bottom: 60px;
  }

  .main-heading {
    font-size: 2.5rem;
  }

  .description-column p {
    font-size: 1.1rem;
  }

  .approach-list li {
    font-size: 1rem;
  }
}
</style>
