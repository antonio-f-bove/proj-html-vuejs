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
      <div class="content-box text-center mb-5">
        <p class="small-text">
          CORPORATE & WEDDINGS
        </p>
        <h3>Baking Special Moments</h3>
      </div>
      <div class="row">
        <div class="img-container col me-5"></div>
        <div class="img-container col ms-5"></div>
      </div>
    </section>

    <section id="products" class="container">
      <div class="row">
        <div class="content-box text-center col-3 me-3">
          <h3 class="mb-3">Find a freshly baked product perfect for you</h3>
          <p class="small-text mb-4">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. At hic voluptatum minima commodi iusto, tempora voluptates ipsam. Odio, impedit? Laborum?
          </p>
          <app-button :theme="'dark'">Shop All Products</app-button>
        </div>
        <div class="slider col">
          <!-- static version -->
          <div class="row">
            <div class="card col">
              <img class="card-img-top" src="/images/choco-chip-cookies.jpg" alt="product">
              <div class="card-body text-center">
                <h6 class="card-title">Choco Chip Cookies</h6>
                <div class="card-text">$19.00 - $39.00</div>
              </div>
            </div>
            <div class="card col">
              <img class="card-img-top" src="/images/choco-chip-cookies.jpg" alt="product">
              <div class="card-body text-center">
                <h6 class="card-title">Choco Chip Cookies</h6>
                <div class="card-text">$19.00 - $39.00</div>
              </div>
            </div>
            <div class="card col">
              <img class="card-img-top" src="/images/choco-chip-cookies.jpg" alt="product">
              <div class="card-body text-center">
                <h6 class="card-title">Choco Chip Cookies</h6>
                <div class="card-text">$19.00 - $39.00</div>
              </div>
            </div>
            <div class="card col">
              <img class="card-img-top" src="/images/choco-chip-cookies.jpg" alt="product">
              <div class="card-body text-center">
                <h6 class="card-title">Choco Chip Cookies</h6>
                <div class="card-text">$19.00 - $39.00</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="process" class="container">
      <div class="box first">
        <div class="overlay">
          <div class="title-container">
            <h2 class="col-5 display-6">Tell us what you have in mind</h2>
            <div class="number display-2">01</div>
          </div>
          <div class="text-container col-4">
            <div class="small-text mb-2">MANUAL INGREDIENTS SELECTION</div>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic porro magnam laboriosam! Molestias cumque, quae blanditiis doloremque amet neque! Voluptatem accusantium quaerat voluptatum quis excepturi delectus a incidunt libero error?</p>
          </div>
        </div>
      </div>
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