<template>
  <div class="head">
    <header>
      <div class="row">
        <div class="logo-container col">
          <img src="/images/avada-bakery-logo.png" alt="logo">
        </div>
        <nav class="col">
          <ul>
            <li>HOME</li>
            <li>HOME</li>
            <li>HOME</li>
          </ul>
        </nav>
      </div>
    </header>
    <div class="jumbo">
      <div class="container">
        <div class="content-box col-4">
          <div class="small-text mb-3">
            FRESH & TASTY EVERY DAY
          </div>
          <h1 class="mb-3">The Perfect Fresh Bread</h1>
          <p class="small-text mb-4">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum consequuntur culpa sunt laudantium recusandae aut pariatur animi, sint quidem magnam error aperiam.
          </p>
          <app-button :theme="'light'">Explore our products</app-button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AppButton from './AppButton.vue'

export default {
  components: { AppButton },
}
</script>

<style lang="scss" scoped>
@import '../style/the-header-style.scss';

</style>