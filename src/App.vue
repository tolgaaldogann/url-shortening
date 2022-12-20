<template>
  <AppHeader/>
  <BannerSection/>
  <StaticsSection/>
  <AppFooter class="footer-section"/>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import BannerSection from './components/BannerSection.vue';
import StaticsSection from './components/StaticsSection.vue';
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    BannerSection,
    StaticsSection,
    AppFooter,
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100%;
  min-height: 100vh;
}
</style>
