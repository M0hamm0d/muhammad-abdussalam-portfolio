<template>
  <section id="skills" class="skills-section">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">My <span class="accent-text">Tech Stack</span></h2>
        <p class="section-subtitle">
          A curated selection of technologies I use to bring digital products to life.
        </p>
      </div>

      <div class="skills-grid">
        <div class="skill-category">
          <div class="category-header">
            <PhDesktop :size="28" weight="duotone" />
            <h3>Frontend Development</h3>
          </div>
          <div class="tags-container">
            <div class="skill-pill">Vue.js</div>
            <div class="skill-pill">React/Next.js</div>
            <div class="skill-pill">JavaScript (ES6+)</div>
            <div class="skill-pill">Pinia / Redux/ Zustand</div>
            <div class="skill-pill">Modern CSS / SCSS</div>
            <div class="skill-pill">Tailwind CSS</div>
          </div>
        </div>

        <div class="skill-category">
          <div class="category-header">
            <PhCloud :size="28" weight="duotone" />
            <h3>Infrastructure & Tools</h3>
          </div>
          <div class="tags-container">
            <div class="skill-pill">Supabase</div>
            <div class="skill-pill">Git / GitHub</div>
            <div class="skill-pill">Vercel / Netlify</div>
            <div class="skill-pill">PostgreSQL</div>
            <div class="skill-pill">RESTful APIs</div>
          </div>
        </div>

        <div class="skill-category">
          <div class="category-header">
            <PhStrategy :size="28" weight="duotone" />
            <h3>Soft Skills & Leadership</h3>
          </div>
          <div class="tags-container">
            <div class="skill-pill">Financial Management</div>
            <div class="skill-pill">Team Leadership</div>
            <div class="skill-pill">Agile Methodology</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { PhDesktop, PhCloud, PhStrategy } from '@phosphor-icons/vue'
</script>
<style scoped>
.skills-section {
  padding: 100px 5%;
  background-color: #f7f1e3; /* Soft Cream */
}

.container {
  max-width: 1100px;
  margin: 0 auto;
}

.section-header {
  margin-bottom: 60px;
}

.section-title {
  font-family: 'Outfit', sans-serif;
  font-size: 2.8rem;
  font-weight: 800;
  color: #2d3436;
}

.accent-text {
  color: #706fd3; /* Tech Violet */
}

.section-subtitle {
  font-family: 'Instrument Sans', sans-serif;
  color: #5d6466;
  margin-top: 10px;
}

/* Skills Grid */
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 30px;
}

.skill-category {
  background: white;
  padding: 40px;
  border-radius: 24px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.02);
  border: 1px solid rgba(112, 111, 211, 0.05);
  transition: all 0.3s ease;
}

.skill-category:hover {
  transform: translateY(-5px);
  border-color: #706fd3;
  box-shadow: 0 10px 30px rgba(112, 111, 211, 0.1);
}

.category-header {
  display: flex;
  align-items: center;
  gap: 15px;
  margin-bottom: 25px;
  color: #706fd3;
}

.category-header h3 {
  font-family: 'Outfit', sans-serif;
  font-size: 1.4rem;
  color: #2d3436;
}

/* Skill Pills */
.tags-container {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.skill-pill {
  font-family: 'Instrument Sans', sans-serif;
  background: #f7f1e3;
  color: #2d3436;
  padding: 8px 16px;
  border-radius: 100px;
  font-size: 0.9rem;
  font-weight: 500;
  border: 1px solid transparent;
  transition: all 0.2s ease;
}

.skill-pill:hover {
  background: #706fd3;
  color: white;
  cursor: default;
}

/* Mobile Adjustments */
@media (max-width: 768px) {
  .section-title {
    font-size: 2.2rem;
  }

  .skill-category {
    padding: 30px;
  }
}
</style>
