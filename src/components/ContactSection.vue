<template>
  <section class="contact">
    <div class="contact-card">
      <h2 class="main-heading">Let's Build Something Together</h2>
      <h3 class="sub-heading">Ready to discuss your next software project?</h3>

      <div class="email-container">
        <a href="mailto:info@anemolabs.de" class="email-link">INFO@ANEMOLABS.DE</a>
        <div class="email-underline"></div>
      </div>

      <div class="contact-details">
        <div class="social-links">
          <a
            href="https://linkedin.com/company/anemolabs"
            target="_blank"
            rel="noopener noreferrer"
            class="social-link"
          >
            LinkedIn
          </a>
          <span class="separator">•</span>
          <a
            href="https://github.com/anemolabs"
            target="_blank"
            rel="noopener noreferrer"
            class="social-link"
          >
            GitHub
          </a>
        </div>

        <div class="location">
          <span>📍 Berlin, Germany</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.contact {
  background-color: var(--color-light-primary);
  padding: 80px 20px 100px;
}

.contact-card {
  background-color: var(--color-white);
  border-radius: 16px;
  padding: 60px;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.08);
  max-width: 900px;
  margin: 0 auto;
}

.main-heading {
  font-size: 2.5rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  margin-bottom: 16px;
  line-height: 1.2;
}

.sub-heading {
  font-size: 1.5rem;
  font-weight: 400;
  color: var(--color-text-primary);
  margin-bottom: 40px;
}

.email-container {
  margin-bottom: 50px;
}

.email-link {
  display: inline-block;
  font-size: 3rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  text-decoration: none;
  letter-spacing: -0.02em;
  transition: color 0.3s ease;
}

.email-link:hover {
  color: var(--color-accent);
}

.email-underline {
  width: 100%;
  height: 3px;
  background-color: var(--color-dark-secondary);
  margin-top: 16px;
  transition: background-color 0.3s ease;
}

.email-link:hover + .email-underline {
  background-color: var(--color-accent);
}

.contact-details {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 20px;
}

.social-links {
  display: flex;
  align-items: center;
  gap: 12px;
}

.social-link {
  font-size: 1rem;
  color: var(--color-text-primary);
  text-decoration: none;
  transition: color 0.3s ease;
}

.social-link:hover {
  color: var(--color-accent);
}

.separator {
  color: var(--color-text-primary);
  opacity: 0.3;
}

.location {
  font-size: 1rem;
  color: var(--color-text-primary);
}

@media (max-width: 768px) {
  .contact-card {
    padding: 40px 30px;
  }

  .main-heading {
    font-size: 1.8rem;
  }

  .sub-heading {
    font-size: 1.2rem;
  }

  .email-link {
    font-size: 1.8rem;
    word-break: break-all;
  }

  .contact-details {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>
