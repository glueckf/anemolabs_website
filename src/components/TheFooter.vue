<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-top">
        <div class="tagline">MODULAR BY NATURE.</div>
        <div class="logo-container">
          <img src="../assets/Logo/Wort-Bildmarke/anemolabs_white.svg" alt="AnemoLabs" class="footer-logo" />
        </div>
      </div>

      <div class="footer-bottom">
        <div class="footer-info">
          <span>Berlin, Germany</span>
          <span class="separator">•</span>
          <span>&copy; 2025</span>
        </div>
        <div class="footer-links">
          <a href="https://linkedin.com/company/anemolabs" target="_blank" rel="noopener noreferrer" class="footer-link">LinkedIn</a>
          <span class="separator">•</span>
          <a href="https://github.com/anemolabs" target="_blank" rel="noopener noreferrer" class="footer-link">Github</a>
          <span class="separator">•</span>
          <a href="#legal" class="footer-link">Legal Notice</a>
          <span class="separator">•</span>
          <a href="#privacy" class="footer-link">Privacy Policy</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
</script>

<style scoped>
.footer {
  background-color: var(--color-dark-primary);
  color: var(--color-text-light);
  padding: 60px 80px 40px;
  margin-top: 80px;
}

.footer-content {
  max-width: 1400px;
  margin: 0 auto;
}

.footer-top {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 60px;
  padding-bottom: 40px;
  border-bottom: 1px solid rgba(255, 255, 255, 0.2);
}

.tagline {
  font-size: 2.5rem;
  font-weight: 600;
  letter-spacing: -0.02em;
  color: var(--color-text-light);
}

.footer-logo {
  height: 50px;
  width: auto;
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 20px;
}

.footer-info {
  display: flex;
  align-items: center;
  gap: 12px;
  font-size: 0.95rem;
  opacity: 0.8;
}

.footer-links {
  display: flex;
  align-items: center;
  gap: 12px;
  font-size: 0.95rem;
}

.footer-link {
  color: var(--color-text-light);
  text-decoration: none;
  opacity: 0.8;
  transition: opacity 0.3s ease;
}

.footer-link:hover {
  opacity: 1;
}

.separator {
  opacity: 0.4;
}

@media (max-width: 768px) {
  .footer {
    padding: 40px 20px 30px;
  }

  .footer-top {
    flex-direction: column;
    align-items: flex-start;
    gap: 30px;
  }

  .tagline {
    font-size: 1.8rem;
  }

  .footer-bottom {
    flex-direction: column;
    align-items: flex-start;
  }

  .footer-links {
    flex-wrap: wrap;
  }
}
</style>
