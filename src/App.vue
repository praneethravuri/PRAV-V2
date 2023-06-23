<template>
  <Navigation />
  <Socials />
  <div class="section-width introduction">
    <Introduction />
  </div>

  <div class="section-width projects">
    <Projects />
  </div>
</template>

<script>

import Navigation from './components/Navigation.vue';
import Socials from './components/Socials.vue';
import Introduction from './components/Introduction.vue';
import Projects from './components/Projects.vue';

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
    Projects
  }
}
</script>

<style lang="scss">
@import "@/styles/main.scss";
</style>
