<template>
  <div class="card">
    <div class="wrapper">
      <div class="overlay">
        <h4>{{ item.name }}</h4>
        <div class="small-text">{{ item.types.join() }}</div>
        <p>{{ item.price }}</p>
      </div>
      <img class="card-img-top" :src="`/images/${item.url}.jpg`" alt="product">
    </div>
    <div v-if="withText" class="card-body text-center">
      <h6 class="card-title">{{ item.name }}</h6>
      <div class="card-text">{{ item.price }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    item: Array,
    withText: Boolean,
  },
  methods: {
    // printTypes (item) {
      
    // }
  }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.card {
  height: 100%;
  border: none;
  position: relative;

  .card-text {
    color: $primary;
  }

  .overlay {
    display: none;
    background-color: #8888;
    // opacity: .4;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    z-index: 1;

    & > * {
      color: #fff;
      z-index: 99;
      position: relative;
    }
  }
  &:hover .overlay {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>