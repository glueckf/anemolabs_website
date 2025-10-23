<template>
  <section class="contact">
    <div class="contact-card">
      <h3 class="sub-heading">Ready to discuss your next software project?</h3>

      <div class="email-container">
        <a href="mailto:info@anemolabs.de" class="email-link">INFO@ANEMOLABS.DE</a>
        <div class="email-underline"></div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.contact {
  background-color: transparent;
  padding: 0;
}

.contact-card {
  background-color: #EBFFF5;
  border-radius: 16px;
  padding: 80px 60px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
}

.sub-heading {
  font-size: 1.5rem;
  font-weight: 400;
  color: var(--color-text-primary);
  margin-bottom: 40px;
}

.email-container {
  margin-bottom: 0;
}

.email-link {
  display: inline-block;
  font-size: 3rem;
  font-weight: 600;
  color: var(--color-dark-primary);
  text-decoration: none;
  letter-spacing: -0.02em;
  transition: color 0.3s ease;
}

.email-link:hover {
  color: var(--color-dark-secondary);
}

.email-underline {
  width: 100%;
  height: 4px;
  background-color: var(--color-dark-primary);
  margin-top: 16px;
  transition: background-color 0.3s ease;
}

.email-link:hover + .email-underline {
  background-color: var(--color-dark-secondary);
}

@media (max-width: 768px) {
  .contact-card {
    padding: 40px 30px;
  }

  .sub-heading {
    font-size: 1.2rem;
  }

  .email-link {
    font-size: 1.8rem;
    word-break: break-all;
  }
}
</style>
