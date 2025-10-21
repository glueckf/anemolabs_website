<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-left">
        <p>&copy; 2025 AnemoLabs</p>
      </div>
      <div class="footer-right">
        <a href="#impressum" class="footer-link">Impressum</a>
        <span class="separator">|</span>
        <a href="#privacy" class="footer-link">Privacy Policy</a>
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
  padding: 40px 20px;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 20px;
}

.footer-left p {
  font-size: 0.95rem;
  opacity: 0.9;
}

.footer-right {
  display: flex;
  align-items: center;
  gap: 16px;
}

.footer-link {
  color: var(--color-text-light);
  text-decoration: none;
  font-size: 0.95rem;
  opacity: 0.9;
  transition: opacity 0.3s ease;
}

.footer-link:hover {
  opacity: 1;
  color: var(--color-accent);
}

.separator {
  opacity: 0.5;
}

@media (max-width: 768px) {
  .footer-content {
    flex-direction: column;
    text-align: center;
  }

  .footer-right {
    justify-content: center;
  }
}
</style>
