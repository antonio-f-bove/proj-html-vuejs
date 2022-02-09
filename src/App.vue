<template>
  <div id="app">
    <the-header />
    <the-main />
    <the-footer />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheMain from './components/TheMain.vue'
import TheFooter from './components/TheFooter.vue'

export default {
  name: "App",
  components: {
    TheHeader,
    TheMain,
    TheFooter,
  },
};
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap.scss';
@import './style/variables.scss';
@import url('https://fonts.googleapis.com/css2?family=Source+Serif+4:wght@400;500;600;700&display=swap');

// utility classes

.small-text {
  font-size: $small-text;
  color: $text-grey;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Source Serif 4', sans-serif;
  font-weight: 600;
  color: $primary; // eccezioni in #process
}
</style>
