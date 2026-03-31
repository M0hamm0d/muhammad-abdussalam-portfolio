<template>
  <nav :class="{ 'nav-scrolled': isScrolled }" class="navbar">
    <div class="nav-container">
      <a href="#hero" class="nav-logo">
        <span class="logo-dot"></span>
        AM
      </a>

      <ul class="nav-links">
        <li><a href="#projects">Projects</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
      </ul>

      <div class="nav-cta">
        <a href="#contact" class="btn-nav-contact">
          Let's Talk
          <PhArrowUpRight :size="16" weight="bold" />
        </a>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'
import { PhArrowUpRight } from '@phosphor-icons/vue'

const isScrolled = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>
<style scoped>
.navbar {
  position: fixed;
  top: 20px;
  left: 0;
  right: 0;
  z-index: 1000;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  padding: 0 5%;
}

.nav-container {
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 12px 24px;
  background: rgba(255, 255, 255, 0.6); /* Glass effect */
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(112, 111, 211, 0.1);
  border-radius: 100px;
}

/* Scroll Animation: Navbar shrinks slightly when scrolling */
.nav-scrolled {
  top: 10px;
}

.nav-scrolled .nav-container {
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
  border-color: rgba(112, 111, 211, 0.3);
}

/* Logo Section */
.nav-logo {
  display: flex;
  align-items: center;
  gap: 8px;
  font-family: 'Outfit', sans-serif;
  font-weight: 800;
  font-size: 1.2rem;
  color: #2d3436;
  text-decoration: none;
}

.logo-dot {
  width: 10px;
  height: 10px;
  background-color: #706fd3; /* Tech Violet */
  border-radius: 50%;
}

/* Nav Links */
.nav-links {
  display: flex;
  list-style: none;
  gap: 30px;
}

.nav-links a {
  text-decoration: none;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.95rem;
  font-weight: 500;
  color: #5d6466;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #706fd3;
}

/* Nav CTA Button */
.btn-nav-contact {
  display: flex;
  align-items: center;
  gap: 8px;
  background: #2d3436;
  color: white;
  padding: 10px 20px;
  border-radius: 100px;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  text-decoration: none;
  transition: all 0.3s ease;
}

.btn-nav-contact:hover {
  background: #706fd3;
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(112, 111, 211, 0.3);
}

/* Smooth Scrolling for the whole page */
html {
  scroll-behavior: smooth;
}

/* Mobile Tweaks */
@media (max-width: 768px) {
  .nav-links {
    display: none; /* Hide links on mobile for simplicity in an urgent build */
  }

  .nav-container {
    padding: 10px 18px;
  }
}
</style>
