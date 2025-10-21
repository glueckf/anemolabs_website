<template>
  <section class="about-us">
    <!-- Main Heading -->
    <h2 class="section-heading">WHO WE ARE</h2>

    <!-- Intro Text -->
    <div class="intro-text">
      <p>
        <span class="highlight">AnemoLabs</span> emerged from a shared vision: building
        high-quality, clean and modern software for businesses. Founded in
        <span class="highlight">2025</span> by two befriended developers who met at TU Berlin,
        we combine technical precision with entrepreneurial drive.
      </p>
    </div>

    <!-- Team Section -->
    <div class="team-grid">
      <div class="team-image">
        <img src="../assets/images/founders.jpg" alt="Founders Robert Kelm and Finn Glück" />
      </div>
      <div class="team-info">
        <h3 class="team-heading">ROBERT KELM & FINN GLÜCK</h3>

        <div class="bio">
          <h4>Robert Kelm - Senior Developer & Frontend Architect</h4>
          <p>
            With years of experience in modern web development, Robert specializes in creating
            elegant, high-performance user interfaces. His expertise in Vue.js, React, and
            TypeScript ensures every project delivers an exceptional user experience. Robert's
            attention to detail and architectural vision drives the frontend excellence at
            AnemoLabs.
          </p>
        </div>

        <div class="bio">
          <h4>Finn Glück - Backend Developer & Integration Specialist</h4>
          <p>
            Finn brings deep expertise in Python, FastAPI, and distributed systems architecture.
            His focus on clean code principles and scalable backend solutions ensures robust,
            maintainable systems. With a strong background in API design and system integration,
            Finn architects the solid foundations that power AnemoLabs solutions.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.about-us {
  background-color: var(--color-light-primary);
}

.section-heading {
  font-size: 1.5rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  margin-bottom: 40px;
  letter-spacing: 0.05em;
}

.intro-text {
  max-width: 900px;
  margin-bottom: 80px;
}

.intro-text p {
  font-size: 1.5rem;
  line-height: 1.8;
  color: var(--color-text-primary);
}

.intro-text .highlight {
  color: var(--color-accent);
  font-weight: 600;
}

.team-grid {
  display: grid;
  grid-template-columns: 1fr 1.5fr;
  gap: 60px;
  align-items: start;
}

.team-image img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.team-heading {
  font-size: 2.5rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  margin-bottom: 40px;
  line-height: 1.2;
  letter-spacing: -0.02em;
}

.bio {
  margin-bottom: 30px;
}

.bio h4 {
  font-size: 1.25rem;
  font-weight: 600;
  color: var(--color-dark-secondary);
  margin-bottom: 12px;
}

.bio p {
  font-size: 1rem;
  line-height: 1.7;
  color: var(--color-text-primary);
}

@media (max-width: 768px) {
  .team-grid {
    grid-template-columns: 1fr;
    gap: 40px;
  }

  .intro-text p {
    font-size: 1.2rem;
  }

  .team-heading {
    font-size: 1.8rem;
  }
}
</style>
