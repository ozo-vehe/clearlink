<script setup>
import AboutSection from './components/AboutSection.vue';
import FaqSection from './components/FaqSection.vue';
import FooterSection from './components/FooterSection.vue';
import HeroSection from './components/HeroSection.vue';
import Navbar from './components/Navbar.vue';
import SocialSection from './components/SocialSection.vue';
import SubscriptionSection from './components/SubscriptionSection.vue';
import TestimonySection from './components/TestimonySection.vue';
import { inject } from '@vercel/analytics/*';
import { onMounted } from 'vue';

omMounted(() => {
  inject()
})
</script>

<template>
  <Navbar />
  <HeroSection />
  <SocialSection />
  <AboutSection />
  <TestimonySection />
  <FaqSection />
  <SubscriptionSection />
  <FooterSection />
</template>

<style scoped>

</style>
