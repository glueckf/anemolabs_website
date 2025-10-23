<template>
  <div class="sticky-logo">
    <!-- This SVG path assumes it's correct based on your original file structure -->
    <img src="../assets/Logo/Bildmarke/anemolabs_abstract_neongreen.svg" alt="AnemoLabs" class="logo" />
  </div>
</template>

<script setup>
// No script needed for this simple component
</script>

<style scoped>
.sticky-logo {
  /* Use position: fixed to keep it on screen during scroll */
  position: fixed;
  /* Align with the 'main' content's padding (40px top, 80px left)
    from App.vue to simulate being in the "1st grid"
  */
  top: 40px;
  left: 80px;
  z-index: 1000;
  /* Make the container invisible so only the logo is "there" */
  background-color: transparent;
}

.logo {
  height: 40px;
  width: auto;
}

/* Adjust for mobile, matching mobile padding from App.vue (20px) */
@media (max-width: 768px) {
  .sticky-logo {
    top: 20px;
    left: 20px;
  }

  .logo {
    height: 32px;
  }
}
</style>
