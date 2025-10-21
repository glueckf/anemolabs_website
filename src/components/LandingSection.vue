<template>
  <section class="landing">
    <div class="background-image"></div>
    <div class="overlay"></div>

    <div class="content">
      <!-- Video Animation -->
      <video
        v-show="showVideo"
        ref="videoRef"
        class="intro-video"
        autoplay
        muted
        playsinline
        @ended="handleVideoEnd"
      >
        <source src="../assets/videos/logoanimation_text_backround.mp4" type="video/mp4" />
      </video>

      <!-- Headline Text (shown after video) -->
      <div v-show="!showVideo" class="headline" :class="{ 'fade-in': !showVideo }">
        <h1>
          Building modular software that flows seamlessly with your business idea.
        </h1>
        <p class="subtitle">
          We craft scalable solutions using modern architecture and clean code principles.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const videoRef = ref(null)
const showVideo = ref(true)

const handleVideoEnd = () => {
  showVideo.value = false
}

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
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  padding: 0;
}

.background-image {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-image: url('../assets/images/trees.jpeg');
  background-size: cover;
  background-position: center;
  filter: blur(4px);
  transform: scale(1.1);
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
  max-width: 80%;
  max-height: 80%;
  object-fit: contain;
}

.headline {
  text-align: center;
  color: var(--color-text-light);
  padding: 0 20px;
  max-width: 900px;
  opacity: 0;
}

.headline.fade-in {
  animation: fadeIn 1.5s ease-in forwards;
}

.headline h1 {
  font-size: 3rem;
  font-weight: 600;
  margin-bottom: 20px;
  line-height: 1.2;
}

.headline .subtitle {
  font-size: 1.5rem;
  font-weight: 300;
  line-height: 1.6;
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}

@media (max-width: 768px) {
  .intro-video {
    max-width: 90%;
    max-height: 60%;
  }

  .headline h1 {
    font-size: 2rem;
  }

  .headline .subtitle {
    font-size: 1.1rem;
  }
}
</style>
