<script setup>
import PortfolioHero from '@/components/PortfolioHero.vue'
import ProjectSections from '../components/ProjectSections.vue'
import AboutMe from '../components/AboutMe.vue'
import MySkills from '../components/MySkills.vue'
import CtaSection from '../components/CtaSection.vue'
import HeaderSection from '@/components/HeaderSection.vue'
</script>
<template>
  <div class="container">
    <HeaderSection />
    <PortfolioHero />
    <ProjectSections />
    <AboutMe />
    <MySkills />
    <CtaSection />
  </div>
</template>
