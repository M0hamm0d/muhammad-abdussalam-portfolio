<template>
  <section class="hero">
    <div class="top-nav">
      <div class="status-pill"><span class="dot"></span> Available for work</div>
      <div class="location-pill">🇳🇬 Ilorin, Nigeria</div>
    </div>

    <div class="main-content">
      <!-- <div class="profile-avatar">
        <img src="/myImage.jpeg" alt="Abdussalam" />
      </div> -->

      <h1 class="headline">
        Frontend developer <br />
        who creates <span class="accent-text">experiences</span>
      </h1>

      <p class="subheadline">
        I build fast, responsive, and user-focused web applications using modern technologies. Open
        to freelance projects, collaborations, and opportunities to create impactful digital
        products.
      </p>

      <div class="cta-group">
        <a href="https://wa.me/2348136208750" target="_blank" class="btn-dark btn-hover">
          <PhPhone :size="20" weight="fill" />
          Call / WhatsApp
        </a>

        <!-- Download Resume Button -->
        <a href="/Abdussalam_Muhammad_Resume.pdf" download class="btn-dark btn-hover">
          <PhFileText :size="20" weight="fill" />
          Download Resume
        </a>
      </div>
    </div>
    <div class="feature-bar">
      <div class="feature-item"><PhCode :size="24" /> High-Performance Websites</div>
      <div class="feature-item"><PhUsers :size="24" /> Client-Focused Approach</div>
      <div class="feature-item">
        <PhChatTeardropDots :size="24" /> Clear & Consistent Communication
      </div>
    </div>
  </section>
</template>

<script setup>
import { PhPhone, PhCode, PhUsers, PhFileText, PhChatTeardropDots } from '@phosphor-icons/vue'
</script>
<style scoped>
/* Option 3: Luxury Tech Duo Import */
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@700;800&family=Instrument+Sans:wght@400;500;600&display=swap');

a {
  text-decoration: none;
}

.hero {
  background-color: #f7f1e3; /* Soft Cream */
  background-image: radial-gradient(#2d3436 0.5px, transparent 0.5px); /* Dot pattern */
  background-size: 24px 24px;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 2rem 5%;
  text-align: center;
  font-family: 'Instrument Sans', sans-serif;
  padding-top: 120px;
}

/* Top Navigation Pills */
.top-nav {
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.status-pill,
.location-pill {
  background: white;
  padding: 8px 16px;
  border-radius: 100px;
  font-size: 14px;
  font-weight: 500;
  display: flex;
  align-items: center;
  gap: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
}

.dot {
  width: 8px;
  height: 8px;
  background-color: #2ecc71;
  border-radius: 50%;
}

/* Profile Avatar */
.profile-avatar img {
  width: 80px;
  height: 80px;
  border-radius: 20px;
  background: #706fd3; /* Tech Violet background */
  margin-bottom: 2rem;
  object-fit: cover;
}

/* Headline & Subheadline */
.headline {
  /* Updated to Outfit */
  font-family: 'Outfit', sans-serif;
  font-size: clamp(2.5rem, 5vw, 4rem);
  font-weight: 800;
  color: #2d3436;
  line-height: 1.1;
  margin-bottom: 1.5rem;
  /* Slightly tighter letter spacing for that luxury look */
  letter-spacing: -0.03em;
}

.accent-text {
  color: #706fd3; /* Tech Violet */
}

.subheadline {
  max-width: 650px;
  color: #5d6466;
  line-height: 1.6;
  margin: 0 auto 2.5rem auto;
  font-size: 1.1rem;
}

/* Buttons */
.cta-group {
  display: flex;
  gap: 1rem;
  justify-content: center;
}

.btn-dark {
  background: #2d3436;
  color: white;
  border: none;
  padding: 14px 28px;
  border-radius: 100px;
  /* Using Outfit for button text makes it pop */
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  display: flex;
  align-items: center;
  gap: 10px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-dark:hover {
  transform: translateY(-2px);
  background: #000000;
}

.btn-white {
  background: white;
  color: #2d3436;
  border: 1px solid rgba(0, 0, 0, 0.1);
  padding: 14px 28px;
  border-radius: 100px;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-white:hover {
  border-color: #706fd3;
  color: #706fd3;
}

/* Resume Button Extra Animation */

/* Fancy Hover Effect for Both Buttons */
.btn-hover {
  position: relative;
  overflow: hidden;
  transition:
    transform 0.3s ease,
    background 0.3s ease;
}

.btn-hover::after {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: rgba(112, 111, 211, 0.2);
  transition: all 0.4s ease;
  border-radius: 100px;
  z-index: 0;
}

.btn-hover:hover::after {
  left: 0;
}

.btn-hover:hover {
  transform: translateY(-2px);
  background: #000;
}

.btn-hover svg,
.btn-hover span {
  position: relative;
  z-index: 1;
}

/* Bottom Feature Bar */
.feature-bar {
  width: 100%;
  max-width: 1100px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  border-top: 1px solid rgba(45, 52, 54, 0.1);
  padding-top: 2rem;
  margin-top: 4rem;
}

.feature-item {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 12px;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  color: #2d3436;
}

/* Mobile Tweaks */
@media (max-width: 768px) {
  .feature-bar {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  .top-nav {
    flex-direction: column;
    align-items: center;
    gap: 10px;
  }
}
</style>
<!-- <style scoped>
@import url("https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@700;800&family=Inter:wght@400;500&display=swap");

.hero {
  background-color: #f7f1e3; /* Soft Cream */
  background-image: radial-gradient(
    #2d3436 0.5px,
    transparent 0.5px
  ); /* Dot pattern */
  background-size: 24px 24px;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 2rem 5%;
  text-align: center;
  font-family: "Inter", sans-serif;
}

/* Top Navigation Pills */
.top-nav {
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.status-pill,
.location-pill {
  background: white;
  padding: 8px 16px;
  border-radius: 100px;
  font-size: 14px;
  font-weight: 500;
  display: flex;
  align-items: center;
  gap: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
}

.dot {
  width: 8px;
  height: 8px;
  background-color: #2ecc71;
  border-radius: 50%;
}

/* Profile Avatar */
.profile-avatar img {
  width: 80px;
  height: 80px;
  border-radius: 20px;
  background: #706fd3; /* Tech Violet background for avatar */
  margin-bottom: 2rem;
  object-fit: cover;
}

/* Headline & Subheadline */
.headline {
  font-family: "Plus Jakarta Sans", sans-serif;
  font-size: clamp(2.5rem, 5vw, 4rem);
  font-weight: 800;
  color: #2d3436;
  line-height: 1.1;
  margin-bottom: 1.5rem;
}

.accent-text {
  color: #706fd3; /* Tech Violet */
}

.subheadline {
  max-width: 650px;
  color: #5d6466;
  line-height: 1.6;
  margin: 0 auto 2.5rem auto;
}

/* Buttons */
.cta-group {
  display: flex;
  gap: 1rem;
  justify-content: center;
}

.btn-dark {
  background: #2d3436;
  color: white;
  border: none;
  padding: 14px 28px;
  border-radius: 100px;
  font-weight: 600;
  display: flex;
  align-items: center;
  gap: 10px;
  cursor: pointer;
}

.btn-white {
  background: white;
  color: #2d3436;
  border: 1px solid rgba(0, 0, 0, 0.1);
  padding: 14px 28px;
  border-radius: 100px;
  font-weight: 600;
  cursor: pointer;
}

/* Bottom Feature Bar */
.feature-bar {
  width: 100%;
  max-width: 1100px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  border-top: 1px solid rgba(45, 52, 54, 0.1);
  padding-top: 2rem;
  margin-top: 4rem;
}

.feature-item {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 12px;
  font-weight: 600;
  color: #2d3436;
}

/* Mobile Tweaks */
@media (max-width: 768px) {
  .feature-bar {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  .top-nav {
    flex-direction: column;
    align-items: center;
    gap: 10px;
  }
}
</style> -->
