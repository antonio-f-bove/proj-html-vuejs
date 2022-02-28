<template>
  <div class="slider">
    <div @click="indexLooper('-')" class="slider-button prev">
      <i class="bi bi-caret-left"></i>
    </div>

    <div class="row g-3" :class="`row-cols-${numberOfCards}`">
       <slider-card v-for="(n, i) in numberOfCards" :key="i" class="col" 
       :item="items[currentIndex + i]" :withText="isCardWithText" 
       />
    </div>

    <div @click="indexLooper('+')" class="slider-button next">
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
    isCardWithText: Boolean,
    items: Array,
  },
  data() {
    return {
      currentIndex: 0,
    }
  },
  methods: { 
    indexLooper (arg) {
      /*
      * qui gestisco l'indice di scorrimento dello slider
      * ho risolto i casi limite ragionando in funzione del 
      numero di slide mostrate in una volta (this.numberOfCards)
      * in questo modo ad ogni click si aggiornano tutte le 
      slide correntemente mostrate

      * rimane un problema da risolvere: nel caso in cui la lista di
      slide da mostrare non è un multiplo del numero di slide mostrate 
      le slide limite non saranno più mostrate se si naviga sempre nella 
      stessa direzzione
      */
      if (arg === '+') {
        this.currentIndex += this.numberOfCards;
      }
      if (arg === '-') {
        this.currentIndex -= this.numberOfCards;
      }

      if (this.currentIndex >= this.items.length) {
        this.currentIndex = 0;
      }
      if (this.currentIndex < 0) {
        this.currentIndex = this.items.length - this.numberOfCards;
      }

      return this.currentIndex
    }
  }
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
    z-index: 100;

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