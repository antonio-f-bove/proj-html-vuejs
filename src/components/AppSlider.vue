<template>
  <div class="slider">
    <div class="slider-button prev">
      <i class="bi bi-caret-left"></i>
    </div>

    <div class="row g-3" :class="`row-cols-${numberOfCards}`">
       <slider-card v-for="n in numberOfCards" :key="n" class="col" 
       :items="items" :withText="isCardWithText" :index="current + n" 
       />
    </div>

    <div @click="current++" class="slider-button next">
      <i class="bi bi-caret-right"></i>
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
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.slider {
  position: relative;

  .slider-button {
    height: 60px;
    width: 30px;
    line-height: 60px;
    text-align: center;
    background-color: $primary;
    opacity: .5;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);

    &.prev {
      left: 0;
    }
    &.next {
      right: 0;
    }

    & i {
      color: #fff;
      font-size: 24px;
    }
  }
}
</style>