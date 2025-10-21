<template>
  <header class="header">
    <div class="header-content">
      <img src="../assets/logos/anemolabs_static_logo.svg" alt="AnemoLabs Logo" class="logo" />
    </div>
  </header>
</template>

<script setup>
</script>

<style scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
  background-color: transparent;
  padding: 20px 40px;
  transition: background-color 0.3s ease;
}

.header.scrolled {
  background-color: rgba(24, 49, 50, 0.95);
  backdrop-filter: blur(10px);
}

.header-content {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  align-items: center;
}

.logo {
  height: 40px;
  width: auto;
}

@media (max-width: 768px) {
  .header {
    padding: 15px 20px;
  }

  .logo {
    height: 32px;
  }
}
</style>
