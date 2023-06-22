<template>
  <Header />
</template>

<script>

import Header from './components/Header.vue';

export default {
  name: 'App',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Header
  }
}
</script>

<style>

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body{
  background-color: #16151d;
  text-decoration: none;
}

</style>
