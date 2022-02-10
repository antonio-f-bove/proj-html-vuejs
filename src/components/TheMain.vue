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
      <div class="row g-4">
        <div class="col-12">
          <div class="large-box first">
            <div class="wrapper">
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
        </div>
        
        <div class="col-6">
          <div class="large-box second">
            <div class="wrapper">
              <div class="title-container">
                <h2 class="col-5 display-6">We Start Baking</h2>
                <div class="number display-2">02</div>
              </div>
              <div class="text-container col-6">
                <div class="small-text mb-2">SWEET AND DELICIOUS</div>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic porro magnam laboriosam! Molestias cumque, quae blanditiis doloremque amet neque! Voluptatem accusantium quaerat voluptatum quis excepturi delectus a incidunt libero error?</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="content-box">
            <div class="small-text mb-5">DON'T JUST TAKE OUR WORD FOR IT</div>
            <h2 class="mb-4">"Finally found an alternative to the mass produced products. Something thatincorporates real organic ingredients, nutrient dense wellness while promoting sustainability and activity"</h2>
            <div class="small-text">Rachel Cooper, Founder</div>
          </div>
        </div>
        <div class="col-12">
          <div class="large-box third">
            <div class="wrapper">
              <div class="title-container">
                <h2 class="col-5 display-6">Delivered to your home</h2>
                <div class="number display-2">03</div>
              </div>
              <div class="text-container col-4">
                <div class="small-text mb-2">BAKED TO ORDER & GIFT WRAPPED</div>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic porro magnam laboriosam! Molestias cumque, quae blanditiis doloremque amet neque! Voluptatem accusantium quaerat voluptatum quis excepturi delectus a incidunt libero error?</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="locations" class="container">
      <div class="content-box text-center">
        <div class="small-text">LOCATIONS</div>
        <h3>Visit our Bakeries</h3>
      </div>
      <div class="d-flex">
        <div class="card">
          <img src="/images/new-york-bk.jpg" alt="new-york" class="card-img-top mb-4">
          <div class="card-body">
            <h4 class="card-title text-center mb-4">New York</h4>
            <div class="row row-cols-4 justify-content-around">
              <div class="small-text text-center">
                <div>CALL US</div>
                <div>1.800.458.556</div>
              </div>
              <div class="small-text text-center">
                <div>OPEN ALL WEEK</div>
                <div>9:00 AM - 6:00 PM</div>
              </div>
              <app-button :theme="'light'" class="text-center">View Map</app-button>
            </div>
          </div>
        </div>
        <div class="card">
          <img src="/images/london-bk.jpg" alt="london" class="card-img-top mb-4">
          <div class="card-body">
            <h4 class="card-title text-center mb-4">London</h4>
            <div class="row row-cols-4 justify-content-around">
              <div class="small-text text-center">
                <div>CALL US</div>
                <div>1.800.458.556</div>
              </div>
              <div class="small-text text-center">
                <div>OPEN ALL WEEK</div>
                <div>9:00 AM - 6:00 PM</div>
              </div>
              <app-button :theme="'light'" class="text-center">View Map</app-button>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="social" class="container">
      <div class="row g-4">
        <div class="col-3"><img class="img-fluid" src="/images/social-1.jpg" alt=""></div>
        <div class="col-6">
          <div class="content-box text-center">
            <div class="small-text mb-3">MADE FOR SHARING</div>
            <h2 class="mb-3">Let's stay in touch</h2>
            <app-button :theme="'dark'">
              <i class="bi bi-instagram"></i> Follow Us
            </app-button>
          </div>
        </div>
        <div class="col-3"><img class="img-fluid" src="/images/social-2.jpg" alt=""></div>
        <div class="col-3"><img class="img-fluid" src="/images/social-3.jpg" alt=""></div>
        <div class="col-3"><img class="img-fluid" src="/images/social-4.jpg" alt=""></div>
        <div class="col-3"><img class="img-fluid" src="/images/social-5.jpg" alt=""></div>
        <div class="col-3"><img class="img-fluid" src="/images/social-6.jpg" alt=""></div>
      </div>
    </section>

    <section id="cta">
      <div class="content-box col-5">
        <div class="small-text mb-3">TRY OUR SEASONAL PRODUCTS</div>
        <h2 class="mb-5">Order for pick-up or delivery to your home</h2>
        <app-button :theme="'light'">Shop Now</app-button>
      </div>
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