<script>
// Import the components
import Navbar from './components/Navbar.vue';
import HeroSection from './components/Hero.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    HeroSection,
  },
};
</script>

<template>
  <div id="app">
    <Navbar />
    <HeroSection />
    <!-- Your other components will go here -->
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
