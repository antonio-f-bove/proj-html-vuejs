<template>
  <footer class="container">
    <div class="row">
      <div class="col-6">
        <div class="footer-left">
          <div class="logo-container mb-4">
            <img class="img-fluid" src="/images/avada-bakery-logo.png" alt="logo">
          </div>
          <nav class="mb-5">
            <ul>
              <li v-for="item in navItems" :key="item">{{ item }}</li>
              <li class="cart"><i class="bi bi-cart-fill"></i><span>0</span></li>
            </ul>
          </nav>
          <div class="small-text">&copy; Copyright 2012 - 2020 Lorem ipsum dolor sit amet consectetur</div>
        </div>
      </div>
      <div class="col-6">
        <div class="footer-right">
          <h5 class="mb-4">Subscribe to our Newsletter</h5>
          <div class="subscribe mb-5">
            <input type="text" placeholder="Enter email address*">
            <app-button class="ms-2" :theme="'dark'">Subscribe</app-button>
          </div>
          <div class="socials">
            <ul>
              <li><i class="bi bi-instagram"></i></li>
              <li><i class="bi bi-twitter"></i></li>
              <li><i class="bi bi-facebook invert-colors"></i></li>
              <li><i class="bi bi-pinterest invert-colors"></i></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import AppButton from './AppButton.vue';

export default {
  components: { AppButton },
  props: {
    navItems: Array,
  }
}
</script>

<style lang="scss" scoped>
@import '../style/the-footer-style.scss';

</style>