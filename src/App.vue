<template>
  <Navigation />
  <Socials />
  <div class="section-width introduction">
    <Introduction />
  </div>
</template>

<script>

import Navigation from './components/Navigation.vue';
import Socials from './components/Socials.vue';
import Introduction from './components/Introduction.vue';

export default {
  name: 'App',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Navigation,
    // eslint-disable-next-line vue/no-unused-components
    Socials,
    // eslint-disable-next-line vue/no-unused-components
    Introduction,
  }
}
</script>

<style lang="scss">
@import "@/styles/main.scss";
</style>
