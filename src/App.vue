<template>
  <Navigation />
  <Socials />
  <div class="section-width">
    <AboutMe />
  </div>
</template>

<script>

import Navigation from './components/Navigation.vue';
import Socials from './components/Socials.vue';
import AboutMe from './components/AboutMe.vue';

export default {
  name: 'App',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Navigation,
    // eslint-disable-next-line vue/no-unused-components
    Socials,
    AboutMe
  }
}
</script>

<style lang="scss">
  @import "@/styles/main.scss";
</style>
