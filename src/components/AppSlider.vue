<template>
  <div class="slider">
    <div class="row g-3" :class="`row-cols-${colsWidth}`">
       <slider-card v-for="n in numberOfCards" :key="n" class="col" :items="items" :withText="isCardWithText" :index="current" />
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
    isCardsWithText: Boolean,
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