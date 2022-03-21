<template>
  <div id="app">
    <the-header :navItems="headerNavList" />
    <the-main :products="products" />
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
  data() {
    return {
      headerNavList: [
        'HOME',
        'SHOP',
        'ABOUT',
        'GALLERY',
        'LOCATIONS',
        'JOURNAL',
        'CONTACT',
        'MY ACCOUNT',
        '<i class="bi bi-cart-fill"></i>',
      ],
      products: [
        {
          "name": "Strawberry Jam Cookies",
          "url": "/strawberry-jam-cookies",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Chocolate Chip Cookies",
          "url": "/choco-chip-cookies",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Blackberry Stuffed Bread",
          "url": "/blackberry-stuffed-bread",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Cookies With Icecream",
          "url": "/cookies-with-ice-cream",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Cherry Cake",
          "url": "/cherry-cake",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Glazed Pancake with Lemon",
          "url": "/glazed-pancake-with-lemon",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Home Bread",
          "url": "/home-bread",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Perfect Macarons",
          "url": "/perfect-macarons",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Premium Bread",
          "url": "/premium-bread",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Small Cupcake",
          "url": "/small-cupcake",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        },
        {
          "name": "Strawberry Donut",
          "url": "/strawberry-donut",
          "price": "$19.00 - $39.00",
          "types": [
            "Cookies",
            "Pastries"
          ]
        }
      ],
    }
  }
};
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap.scss';
@import '~bootstrap-icons/font/bootstrap-icons.css';
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
