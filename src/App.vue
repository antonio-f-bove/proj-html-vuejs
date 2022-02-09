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

// utility classes

.small-text {
  font-size: .8rem;
}
</style>
