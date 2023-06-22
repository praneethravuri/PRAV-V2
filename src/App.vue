<template>
  <Navigation />
</template>

<script>

import Navigation from './components/Navigation.vue';

export default {
  name: 'App',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Navigation
  }
}
</script>

<style lang="scss">
  @import "@/styles/main.scss";
</style>
