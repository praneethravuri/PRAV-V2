<template>
  <Navigation />
  <Socials />
</template>

<script>

import Navigation from './components/Navigation.vue';
import Socials from './components/Socials.vue';

export default {
  name: 'App',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Navigation,
    // eslint-disable-next-line vue/no-unused-components
    Socials
  }
}
</script>

<style lang="scss">
  @import "@/styles/main.scss";
</style>
