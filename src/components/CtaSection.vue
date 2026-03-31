<template>
  <section id="contact" class="cta-section">
    <div class="container">
      <div class="cta-card">
        <div class="cta-content">
          <h2 class="cta-title">
            Ready to build something
            <span class="accent-text">extraordinary?</span>
          </h2>
          <p class="cta-subtitle">
            I'm currently looking for new opportunities. Whether you have a question or just want to
            say hi, my inbox is always open.
          </p>

          <div class="cta-actions">
            <a href="mailto:masalami042@gmail.com" class="btn-email">
              <PhEnvelopeSimple :size="24" weight="bold" />
              Send an Email
            </a>
            <div class="social-links">
              <a
                href="https://www.linkedin.com/in/muhammad-abdussalam-7b5102319"
                class="social-icon"
                ><PhLinkedinLogo :size="28"
              /></a>
              <a href="https://github.com/M0hamm0d" class="social-icon"
                ><PhGithubLogo :size="28"
              /></a>
              <a href="https://x.com/masalami0042" class="social-icon"
                ><PhTwitterLogo :size="28"
              /></a>
            </div>
          </div>
        </div>
      </div>

      <footer class="mini-footer">
        <p>&copy; 2026 Abdussalam Muhammad. Turning ideas into digital experiences.</p>
        <p class="location-tag">Let’s build something great</p>
      </footer>
    </div>
  </section>
</template>

<script setup>
import { PhEnvelopeSimple, PhLinkedinLogo, PhGithubLogo, PhTwitterLogo } from '@phosphor-icons/vue'
</script>
<style scoped>
.cta-section {
  padding: 70px 5% 40px 5%;
  background-color: #f7f1e3; /* Matches your background */
}

.container {
  max-width: 1100px;
  margin: 0 auto;
}

.cta-card {
  background-color: #2d3436; /* Dark Anthracite */
  padding: 80px 40px;
  border-radius: 40px;
  text-align: center;
  position: relative;
  overflow: hidden;
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
}

/* Subtle background glow effect */
.cta-card::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, rgba(112, 111, 211, 0.1) 0%, transparent 70%);
  pointer-events: none;
}

.cta-title {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(2rem, 4vw, 3.5rem);
  color: #f5f5f5;
  font-weight: 800;
  margin-bottom: 20px;
  line-height: 1.2;
}

.accent-text {
  color: #706fd3; /* Tech Violet */
}

.cta-subtitle {
  font-family: 'Instrument Sans', sans-serif;
  color: #a0a0a0;
  max-width: 600px;
  margin: 0 auto 40px auto;
  font-size: 1.1rem;
  line-height: 1.6;
}

.cta-actions {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 30px;
}

.btn-email {
  background-color: #706fd3;
  color: white;
  padding: 18px 40px;
  border-radius: 100px;
  font-family: 'Outfit', sans-serif;
  font-weight: 700;
  font-size: 1.1rem;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 12px;
  transition: all 0.3s ease;
  box-shadow: 0 10px 20px rgba(112, 111, 211, 0.3);
}

.btn-email:hover {
  transform: translateY(-5px);
  background-color: #5d5cb3;
  box-shadow: 0 15px 30px rgba(112, 111, 211, 0.4);
}

.social-links {
  display: flex;
  gap: 25px;
}

.social-icon {
  color: #a0a0a0;
  transition:
    color 0.3s ease,
    transform 0.3s ease;
}

.social-icon:hover {
  color: #706fd3;
  transform: scale(1.2);
}

/* Footer Styling */
.mini-footer {
  margin-top: 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.9rem;
  color: #5d6466;
  border-top: 1px solid rgba(45, 52, 54, 0.1);
  padding-top: 30px;
}

.location-tag {
  font-weight: 600;
}

/* Mobile Tweaks */
@media (max-width: 768px) {
  .cta-card {
    padding: 60px 20px;
    border-radius: 30px;
  }

  .mini-footer {
    flex-direction: column;
    gap: 15px;
    text-align: center;
  }
}
</style>
