<template>
  <section class="landing">
    <!-- This background will show if the video fails to load -->
    <div class="background-image"></div>
    <div class="overlay"></div>

    <div class="content">
      <!--
        Video Animation
        - Removed 'loop' attribute.
        - Removed '@ended' handler and 'showVideo' logic.
        - The video will now play once and stop, showing the last frame.

        *** IMPORTANT ***
        The video file '../assets/Animationen/logoanimation_text_backround.mp4'
        was NOT in the uploaded file list. If this file is missing, the
        video will not play, and only the dark background will be visible.
      -->
      <video
        ref="videoRef"
        class="intro-video"
        autoplay
        muted
        playsinline
      >
        <source src="../assets/Animationen/logoanimation_text_backround.mp4" type="video/mp4" />
      </video>

      <!--
        Headline Text (REMOVED)
        Per your request, I've removed the headline text
        so only the video is shown.
      -->
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const videoRef = ref(null)

// Just play the video on mount
onMounted(() => {
  if (videoRef.value) {
    videoRef.value.play()
  }
})
</script>

<style scoped>
.landing {
  position: relative;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  padding: 0 !important;
  margin: 0;
  /* These margins pull the section to the full screen edge */
  margin-left: -80px;
  margin-right: -80px;
  margin-top: -40px;
  margin-bottom: 40px;
}

.background-image {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #183132;
  background-size: cover;
  background-position: center;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.4);
}

.content {
  position: relative;
  z-index: 10;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.intro-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Removed headline styles as it's no longer present */

@media (max-width: 768px) {
  .landing {
    margin-left: -20px;
    margin-right: -20px;
    margin-top: -20px;
  }
}
</style>
