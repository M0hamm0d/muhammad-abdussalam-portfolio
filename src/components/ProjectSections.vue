<template>
  <section id="projects" class="projects-section">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Selected <span class="accent-text">Works</span></h2>
        <p class="section-subtitle">
          A collection of web applications built with precision and modern frontend architecture.
        </p>
      </div>

      <div class="projects-grid">
        <div class="project-card">
          <div class="image-container">
            <img
              src="/univent-pages.jpg"
              width="600"
              height="400"
              alt="UniVent App"
              class="project-img"
            />
            <div class="overlay">
              <div class="overlay-buttons">
                <a href="https://univent.website" class="btn-live"
                  ><PhGlobe :size="20" /> Live Demo</a
                >
                <a href="https://github.com/M0hamm0d/univent-event-application" class="btn-git"
                  ><PhGithubLogo :size="20" /> GitHub</a
                >
              </div>
            </div>
          </div>
          <div class="project-info">
            <div class="tech-stack">
              <span>Vue.js</span>
              <span>Supabase</span>
              <span>Pinia</span>
            </div>
            <h3 class="project-name">UniVent</h3>
            <p class="project-desc">
              A centralized campus event platform for University of Ilorin students, making it easy
              to discover, track, and stay updated on events across campus while helping organizers
              reach more students.
            </p>
            <div class="mobile-actions">
              <a href="https://univent.website" class="btn-live-sm"><PhGlobe :size="18" /> Demo</a>
              <a href="https://github.com/M0hamm0d/univent-event-application" class="btn-git-sm"
                ><PhGithubLogo :size="18" /> Code</a
              >
            </div>
          </div>
        </div>

        <div class="project-card">
          <div class="image-container">
            <img
              src="/kirah-1.png"
              alt="Kirah's Treat"
              width="600"
              height="400"
              class="project-img"
            />
            <div class="overlay">
              <div class="overlay-buttons">
                <a href="https://kirahs-treat-website.vercel.app/" class="btn-live"
                  ><PhGlobe :size="20" /> Live Demo</a
                >
                <a href="https://github.com/M0hamm0d/kirahs-treat-website" class="btn-git"
                  ><PhGithubLogo :size="20" /> GitHub</a
                >
              </div>
            </div>
          </div>
          <div class="project-info">
            <div class="tech-stack">
              <span>Vue.js</span>
              <span>Supabase</span>
              <span>Pinia</span>
            </div>
            <h3 class="project-name">Kirah’s Treat</h3>
            <p class="project-desc">
              A dessert brand focused on creating fresh, high-quality cakes, pastries, and treats
              that combine great taste with beautiful presentation for every occasion.
            </p>
            <div class="mobile-actions">
              <a href="https://kirahs-treat-website.vercel.app/" class="btn-live-sm"
                ><PhGlobe :size="18" /> Demo</a
              >
              <a href="https://github.com/M0hamm0d/kirahs-treat-website" class="btn-git-sm"
                ><PhGithubLogo :size="18" /> Code</a
              >
            </div>
          </div>
        </div>
        <div class="project-card">
          <div class="image-container">
            <img
              src="/rightcare.png"
              alt="right care"
              width="600"
              height="400"
              class="project-img"
            />
            <div class="overlay">
              <div class="overlay-buttons">
                <a href="https://www.rightcarefinder.co.uk/" class="btn-live"
                  ><PhGlobe :size="20" /> Live Demo</a
                >
                <a href="https://github.com/RogueDevTech/right-care-finder" class="btn-git"
                  ><PhGithubLogo :size="20" /> GitHub</a
                >
              </div>
            </div>
          </div>
          <div class="project-info">
            <div class="tech-stack">
              <span>TypeScript</span>
              <span>Next.js</span>
              <span>SCSS</span>
              <span>Zustand</span>
            </div>
            <h3 class="project-name">Right Care Finder</h3>
            <p class="project-desc">
              Collaborated with a team to build a care home discovery platform that helps families
              quickly find and compare care homes across the UK by location, care type, and reviews.
            </p>
            <div class="mobile-actions">
              <a href="https://www.rightcarefinder.co.uk/" class="btn-live-sm"
                ><PhGlobe :size="18" /> Demo</a
              >
              <a href="https://github.com/RogueDevTech/right-care-finder" class="btn-git-sm"
                ><PhGithubLogo :size="18" /> Code</a
              >
            </div>
          </div>
        </div>
        <div class="project-card">
          <div class="image-container">
            <img
              src="/voltedge.png"
              alt="voltedge technology"
              width="600"
              height="400"
              class="project-img"
            />
            <div class="overlay">
              <div class="overlay-buttons">
                <a href="https://voltedge-technology.vercel.app/" class="btn-live"
                  ><PhGlobe :size="20" /> Live Demo</a
                >
                <a href="https://github.com/M0hamm0d/voltedge-technology" class="btn-git"
                  ><PhGithubLogo :size="20" /> GitHub</a
                >
              </div>
            </div>
          </div>
          <div class="project-info">
            <div class="tech-stack">
              <span>Vue.js</span>
              <span>Supabase</span>
              <span>Pinia</span>
            </div>
            <h3 class="project-name">VoltEdge Technologies</h3>
            <p class="project-desc">
              A modern gadget retail platform currently in development, focused on delivering
              cutting-edge electronics through a sleek, user-friendly experience for students and
              tech enthusiasts.
            </p>
            <div class="mobile-actions">
              <a href="https://voltedge-technology.vercel.app/" class="btn-live-sm"
                ><PhGlobe :size="18" /> Demo</a
              >
              <a href="https://github.com/M0hamm0d/voltedge-technology" class="btn-git-sm"
                ><PhGithubLogo :size="18" /> Code</a
              >
            </div>
          </div>
        </div>
      </div>

      <div class="section-footer">
        <a href="https://github.com/M0hamm0d" target="_blank" class="btn-view-all">
          View All Projects on GitHub
          <PhArrowRight :size="20" />
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
import { PhGlobe, PhGithubLogo, PhArrowRight } from '@phosphor-icons/vue'
</script>
<style scoped>
.projects-section {
  padding: 80px 5%;
  background-color: #f7f1e3;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

.section-header {
  margin-bottom: 50px;
  text-align: left;
}

.section-title {
  font-family: 'Outfit', sans-serif;
  font-size: 2.5rem;
  color: #2d3436;
  font-weight: 800;
}

.section-subtitle {
  font-family: 'Instrument Sans', sans-serif;
  color: #5d6466;
  max-width: 500px;
  margin-top: 10px;
}

/* Grid Layout */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
  gap: 30px;
}

/* Card Styling */
.project-card {
  background: white;
  border-radius: 24px;
  overflow: hidden;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.03);
  transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.project-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 20px 40px rgba(112, 111, 211, 0.15);
}

/* Image & Overlay */
.image-container {
  position: relative;
  width: 100%;
  height: 250px;
  overflow: hidden;
}

.project-img {
  width: 100%;
  height: 100%;
  object-fit: fill;
  transition: transform 0.5s ease;
}

.project-card:hover .project-img {
  transform: scale(1.1);
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(45, 52, 54, 0.8); /* Dark Anthracite */
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0;
  transition: opacity 0.3s ease;
  backdrop-filter: blur(4px);
}

.project-card:hover .overlay {
  opacity: 1;
}

.overlay-buttons {
  display: flex;
  gap: 15px;
}

/* Overlay Button Styles */
.btn-live,
.btn-git {
  padding: 10px 20px;
  border-radius: 50px;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  text-decoration: none;
  font-size: 0.9rem;
  display: flex;
  align-items: center;
  gap: 8px;
  transition: all 0.2s ease;
}

.btn-live {
  background: #706fd3;
  color: white;
}

.btn-git {
  background: white;
  color: #2d3436;
}

.btn-live:hover,
.btn-git:hover {
  transform: scale(1.05);
}

/* Text Info Area */
.project-info {
  padding: 25px;
  text-align: left;
}

.tech-stack {
  display: flex;
  gap: 10px;
  margin-bottom: 15px;
}

.tech-stack span {
  font-size: 0.75rem;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  color: #706fd3;
  background: rgba(112, 111, 211, 0.1);
  padding: 4px 12px;
  border-radius: 100px;
  text-transform: uppercase;
}

.project-name {
  font-family: 'Outfit', sans-serif;
  font-size: 1.5rem;
  color: #2d3436;
  margin-bottom: 10px;
}

.project-desc {
  font-family: 'Instrument Sans', sans-serif;
  color: #5d6466;
  line-height: 1.5;
  font-size: 0.95rem;
}

/* Mobile Tweak */
@media (max-width: 500px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }
}

.section-footer {
  margin-top: 60px;
  display: flex;
  justify-content: center;
}

.btn-view-all {
  display: flex;
  align-items: center;
  gap: 12px;
  background-color: #2d3436;
  color: #ffffff;
  padding: 16px 32px;
  border-radius: 100px;
  text-decoration: none;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  transition: all 0.3s ease;
}

.btn-view-all:hover {
  background-color: #706fd3;
  transform: scale(1.05);
}

/* Hide Mobile Actions by default (Desktop) */
.mobile-actions {
  display: none;
  gap: 10px;
  margin-top: 20px;
}

.btn-live-sm,
.btn-git-sm {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 6px;
  padding: 10px;
  border-radius: 12px;
  font-size: 0.85rem;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  text-decoration: none;
}

.btn-live-sm {
  background: #706fd3;
  color: white;
}
.btn-git-sm {
  background: #f0f0f0;
  color: #2d3436;
}

/* Responsive Adjustments */
@media (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }

  /* Disable Overlay on Mobile */
  .overlay {
    display: none;
  }

  .project-card:hover {
    transform: none; /* Less jarring on mobile tap */
  }

  .project-card:hover .project-img {
    transform: none;
  }

  /* Show Mobile Buttons */
  .mobile-actions {
    display: flex;
  }

  .section-title {
    font-size: 2rem;
  }
}

@media (max-width: 500px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }
}
</style>
