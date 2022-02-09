<template>
  <main>

    <section id="start-shopping" class="container">
      <div class="row">
        <div class="content-box col-4">
          <p class="small-text">OUR PRODUCTS</p>
          <h3 class="mb-5">All our delectable pastries are baked fresh in our Kitchen every morning, and are made with all-natural, all organic ingredients</h3>
          <app-button :theme="'dark'">Start Shopping</app-button>
        </div>
        <div class="slider col">
          <!-- static version -->
          <!-- TODO: prev&next buttons -->
          <div class="row">
            <div class="img-container col-6 ps-4">
              <img class="img-fluid" src="/images/choco-chip-cookies.jpg" alt="cookies">
            </div>
            <div class="img-container col-6 pe-4">
              <img class="img-fluid" src="/images/strawberry-jam-cookies.jpg" alt="cookies">
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="special-moments" class="container">

    </section>

    <section id="products" class="container">

    </section>

    <section id="process" class="container">

    </section>

    <section id="locations" class="container">

    </section>

    <section id="social" class="container">

    </section>

    <section id="cta">
      <div class="content-box"></div>
    </section>
  </main>
</template>

<script>
import AppButton from './AppButton.vue'

export default {
  components: { AppButton },
  
}
</script>

<style lang="scss" scoped>
@import '../style/the-main-style.scss';
</style>