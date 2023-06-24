<template>
  <Navigation />
  <Socials />
  <div class="section-width introduction">
    <Introduction />
  </div>

  <div class="section-width projects">
    <Projects />
  </div>

  <div class="section-width experience">
    <Experience />
  </div>

  <div class="section-width experience">
    <Contact />
  </div>
</template>

<script>

import Navigation from './components/Navigation.vue';
import Socials from './components/Socials.vue';
import Introduction from './components/Introduction.vue';
import Projects from './components/Projects.vue';
import Experience from './components/Experience.vue';
import Contact from './components/Contact.vue';

export default {
  name: 'App',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Navigation,
    // eslint-disable-next-line vue/no-unused-components
    Socials,
    // eslint-disable-next-line vue/no-unused-components
    Introduction,
    // eslint-disable-next-line vue/no-unused-components
    Projects,
    // eslint-disable-next-line vue/no-unused-components
    Experience,
    // eslint-disable-next-line vue/no-unused-components
    Contact
  }
}
</script>

<style lang="scss">
@import "@/styles/main.scss";
</style>
