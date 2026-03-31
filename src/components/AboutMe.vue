<template>
  <section id="about" class="about-section">
    <div class="container">
      <div class="about-grid">
        <div class="about-visual">
          <div class="image-wrapper">
            <img src="/myImage.jpeg" alt="Abdussalam Muhammad" />
            <div class="experience-badge">
              <span class="number">3+</span>
              <span class="label">Years of <br />Coding</span>
            </div>
          </div>
        </div>

        <div class="about-content">
          <h2 class="section-title">A little about <span class="accent-text">me</span></h2>

          <div class="bio-text">
            <p>
              Hi, I am Muhammad Abdussalam. A frontend developer and Computer Engineering student at
              the University of Ilorin, focused on building fast, scalable, and visually engaging
              web applications using Vue.js, JavaScript, and modern CSS architecture.
            </p>
            <p>
              I specialize in turning complex ideas into clean, intuitive user experiences. From
              building platforms like UniVent to crafting responsive and high-performing interfaces,
              my goal is to create products that are not only functional, but also seamless and
              enjoyable to use.
            </p>
            <p>
              Beyond development, I bring strong organization and leadership experience. I currently
              serve as the Financial Secretary of The Dawn (Kwara District), a faith-based,
              non-governmental organization, and I am also the former Program Director. In these
              roles, I have contributed to planning, coordinating, and executing impactful,
              community-driven initiatives.
            </p>
          </div>
          <div class="skills-mini-grid">
            <div class="skill-tag"><PhDeviceMobile :size="20" /> Responsive Design</div>
            <div class="skill-tag"><PhGithubLogo :size="20" /> Version Control (Git)</div>
            <div class="skill-tag"><PhUsersThree :size="20" /> Team Collaboration</div>
            <div class="skill-tag"><PhRocketLaunch :size="20" /> Project Delivery</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { PhUsersThree, PhGithubLogo, PhDeviceMobile, PhRocketLaunch } from '@phosphor-icons/vue'
</script>
<style scoped>
.about-section {
  padding: 20px 5%;
  background-color: #f7f1e3;
}

.container {
  max-width: 1100px;
  margin: 0 auto;
}

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1.2fr;
  gap: 80px;
  align-items: center;
}

/* Visual Side */
.image-wrapper {
  position: relative;
  border-radius: 30px;
  background: #706fd3;
  padding: 10px;
}

.image-wrapper img {
  width: 100%;
  height: auto;
  border-radius: 20px;
  display: block;
  /* filter: grayscale(0%); */
  /* transition: filter 0.3s ease; */
}

/* .image-wrapper:hover img {
  filter: grayscale(0%);
} */

.experience-badge {
  position: absolute;
  bottom: -20px;
  right: -20px;
  background: #2d3436;
  color: white;
  padding: 20px;
  border-radius: 20px;
  display: flex;
  align-items: center;
  gap: 12px;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
}

.experience-badge .number {
  font-family: 'Outfit', sans-serif;
  font-size: 2rem;
  font-weight: 800;
  color: #706fd3;
}

.experience-badge .label {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.8rem;
  line-height: 1.2;
  text-transform: uppercase;
  letter-spacing: 1px;
}

/* Content Side */
.section-title {
  font-family: 'Outfit', sans-serif;
  font-size: 2.8rem;
  font-weight: 800;
  color: #2d3436;
  margin-bottom: 30px;
}

.accent-text {
  color: #706fd3;
}

.bio-text p {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 1.1rem;
  color: #5d6466;
  line-height: 1.8;
  margin-bottom: 20px;
}

.bio-text strong {
  color: #2d3436;
  font-weight: 600;
}

/* Skills Tags */
.skills-mini-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 15px;
  margin-top: 40px;
}

.skill-tag {
  background: white;
  padding: 12px 20px;
  border-radius: 12px;
  display: flex;
  align-items: center;
  gap: 10px;
  font-family: 'Outfit', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  color: #2d3436;
  border: 1px solid rgba(112, 111, 211, 0.1);
}

/* Mobile Responsiveness */
@media (max-width: 900px) {
  .about-grid {
    grid-template-columns: 1fr;
    gap: 60px;
    text-align: center;
  }

  .about-visual {
    max-width: 400px;
    margin: 0 auto;
  }

  .skills-mini-grid {
    grid-template-columns: 1fr;
  }

  .skill-tag {
    justify-content: center;
  }
}
</style>
