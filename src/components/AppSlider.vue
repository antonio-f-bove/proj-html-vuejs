<template>
  <div class="slider">
    <div class="slider-button prev"
    @click="decrementCurrent"
    >
      <i class="bi bi-chevron-left"></i>
    </div>

    <div v-if="cardWithText"
    class="d-flex"
    >
      <slider-card-2 v-for="i in outputSlides" :key="i" 
      :item="items[(current + i) % items.length]"
      class="custom-margin"
      />
    </div>
    <div v-if="!cardWithText"
    class="d-flex"
    >
      <slider-card-1 v-for="i in outputSlides" :key="i" 
      :item="items[(current + i) % items.length]"
      class="custom-margin"
      />
    </div>

    <div class="slider-button next"
    @click="incrementCurrent"
    >
      <i class="bi bi-chevron-right"></i>
    </div>
  </div>
</template>

<script>
import SliderCard1 from './SliderCard1.vue'
import SliderCard2 from './SliderCard2.vue';

export default {
  components: { 
    SliderCard1,
    SliderCard2,
    },
  props: {
    items: Array,
    cardWithText: Boolean,
    outputSlides: Number,
  },
  data() {
    return {
      current: 0,
    }
  },
  methods: {
    incrementCurrent() {
      this.current++;
    },
    decrementCurrent() {
      this.current--;

      if (this.current < 0) {
        this.current = this.items.length - 1;
      }
    },
  }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.slider {
  position: relative;

  .slider-button {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    z-index: 99;
    height: 12%;
    padding: 0 .4em;
    font-size: .8em;
    color: #fff;
    background-color: $primary;
    opacity: .6;
    display: flex;
    align-items: center;
    cursor: pointer;

    &.prev {
      left: 0;
    }
    &.next {
      right: 0;
    }
  }

  .custom-margin {
    margin: 0 .4em;
    &:first-child {
      margin-left: 0;
    }
    &:last-child {
      margin-right: 0;
    }
  }
}
</style>