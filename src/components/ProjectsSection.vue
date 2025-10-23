<template>
  <section class="projects">
    <div class="content-card">
      <h2 class="section-heading">OUR PROJECTS</h2>

      <div class="development-notice">
        <h3 class="sub-heading">
          CURRENTLY IN DEVELOPMENT<span class="asterisk">*</span>
        </h3>
        <p class="description">
          We're currently crafting our first major client project – a sophisticated AI powered
          solution that demonstrates our full technical capabilities.
        </p>
        <p class="coming-soon">More details coming soon.</p>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.projects {
  background-color: transparent;
}

.section-heading {
  font-size: 1.125rem;
  font-weight: 600;
  color: var(--color-text-primary);
  margin-bottom: 30px;
  letter-spacing: 0.05em;
}

.development-notice {
  max-width: 800px;
}

.sub-heading {
  font-size: 2rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  margin-bottom: 24px;
  letter-spacing: 0.02em;
}

.asterisk {
  color: var(--color-accent);
  font-size: 2.5rem;
  margin-left: 4px;
}

.description {
  font-size: 1.25rem;
  line-height: 1.8;
  color: var(--color-text-primary);
  margin-bottom: 16px;
}

.coming-soon {
  font-size: 1.1rem;
  color: var(--color-text-primary);
  font-style: italic;
  opacity: 0.8;
}

@media (max-width: 768px) {
  .sub-heading {
    font-size: 1.5rem;
  }

  .asterisk {
    font-size: 2rem;
  }

  .description {
    font-size: 1.1rem;
  }
}
</style>
