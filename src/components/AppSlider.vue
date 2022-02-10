<template>
  <div class="slider">
    <div class="row g-3" :class="`row-cols-${colsWidth}`">
       <div v-for="(item, i) in items" :key="item" class="col">
         <div v-if="i >= current && i < current + numberOfCards" 
         class="card"
         >
            <img class="card-img-top" :src="`/images${item}.jpg`" alt="product">
            <div class="card-body text-center">
              <h6 class="card-title">Choco Chip Cookies</h6>
              <div class="card-text">$19.00 - $39.00</div>
            </div>
          </div>
       </div>
    </div>
  </div>
</template>

<script>
import SliderCard from './SliderCard.vue'

export default {
  components: {
    SliderCard
  },
  props: {
    numberOfCards: Number,
    cardsWithText: Boolean,
    items: Array,
  },
  data() {
    return {
      current: 0,
    }
  },
  computed: {
    colsWidth () {
      return 12 / this.numberOfCards
    }
  }
}
</script>

<style lang="scss" scoped>

</style>