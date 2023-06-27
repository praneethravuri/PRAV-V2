<template>
  <div id="navigation">
    <Navigation />
  </div>

  <Socials />

  <div class="main-content">

    <div class="section-width introduction">
      <Introduction />
    </div>

    <div class="section-width" id="about">
      <About />
    </div>

    <div class="section-width experience" id="experience">
      <Experience />
    </div>

    <div class="section-width projects" id="projects">
      <Projects />
    </div>

    <div class="section-width" id="contact">
      <Contact />
    </div>

    <div class="section-width" style="padding: 0;">
      <Footer />
    </div>
  </div>
</template>

<script>

import Navigation from './components/Navigation.vue';
import Socials from './components/Socials.vue';
import About from './components/About.vue';
import Introduction from './components/Introduction.vue';
import Projects from './components/Projects.vue';
import Experience from './components/Experience.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';

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
    About,
    // eslint-disable-next-line vue/no-unused-components
    Projects,
    // eslint-disable-next-line vue/no-unused-components
    Experience,
    // eslint-disable-next-line vue/no-unused-components
    Contact,
    // eslint-disable-next-line vue/no-unused-components
    Footer
  }
}
</script>

<style lang="scss">
@import "@/styles/main.scss";
</style>
