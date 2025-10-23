<template>
  <section class="what-we-do">
    <div class="content-card">
      <!-- Section Label -->
      <div class="section-label">WHAT WE DO</div>

      <!-- Top Grid: Heading and Description -->
      <div class="top-grid">
        <div class="heading-column">
          <h2 class="main-heading">SOFTWARE THAT FLOWS</h2>
        </div>
        <div class="description-column">
          <p>
            We specialise in creating custom software solutions that are designed with performance, scalability and maintainability in mind. Each project adheres to industry best practices, with a particular emphasis on clean architecture.
          </p>
        </div>
      </div>

      <!-- Bottom Section: Our Approach -->
      <div class="approach-section">
        <h3 class="approach-heading">OUR APPROACH</h3>
        <ul class="approach-list">
          <li class="approach-item">
            <span class="number">01</span>
            <span class="text">Modular systems that adapt to your growing needs</span>
          </li>
          <li class="approach-item">
            <span class="number">02</span>
            <span class="text">Modern tech stack: Vue.js, FastAPI, Python, Docker</span>
          </li>
          <li class="approach-item">
            <span class="number">03</span>
            <span class="text">Comprehensive testing and documentation</span>
          </li>
          <li class="approach-item">
            <span class="number">04</span>
            <span class="text">Seamless integrations (APIs, AI tools, legacy systems)</span>
          </li>
          <li class="approach-item last">
            <span class="number">05</span>
            <span class="text">Future-proof architecture that scales with your business</span>
          </li>
        </ul>

        <!-- Tech Logos -->
        <TechCarousel />
      </div>
    </div>
  </section>
</template>

<script setup>
import TechCarousel from './TechCarousel.vue'
</script>

<style scoped>
.what-we-do {
  background-color: transparent;
}

.section-label {
  font-size: 0.875rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  color: var(--color-text-primary);
  margin-bottom: 30px;
}

.top-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 60px;
  margin-bottom: 50px;
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
  margin-top: 0;
  padding-top: 40px;
  border-top: 1px solid #e0e0e0;
}

.approach-heading {
  font-size: 1.125rem;
  font-weight: 600;
  color: var(--color-text-primary);
  margin-bottom: 30px;
  letter-spacing: 0.05em;
}

.approach-list {
  list-style: none;
  padding: 0;
  margin-bottom: 50px;
}

.approach-item {
  display: flex;
  align-items: baseline;
  gap: 20px;
  padding: 20px 0;
  font-size: 1rem;
  border-bottom: 1px solid #d0d0d0;
}

.approach-item.last {
  border-bottom: none;
}

.approach-list .number {
  font-size: 0.875rem;
  font-weight: 600;
  font-style: italic;
  color: var(--color-text-primary);
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
