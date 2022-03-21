<template>
  <div class="card">
    <div class="wrapper">
      <div class="overlay px-3">
        <p class="small-text">SELECT OPTIONS  /  QUICK VIEW</p>
      </div>
      <img class="card-img-top" :src="`/images/${item.url}.jpg`" alt="product">
    </div>
    <div class="card-body text-center">
      <h6 class="card-title">{{ item.name }}</h6>
      <div class="card-text small-text">{{ item.price }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    item: Object,
  },
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.card {
  height: 100%;
  border: none;
  position: relative;

  /*
  consflitto con il componente card di bootstrap per la centratura
  del testo nell'overlay. Non ho trovato una soluzione che non comprendesse 
  rifare la card da capo. Piccolo workaround su card-body col z-index, che gli 
  permette di stare al di siopra dell'overlay
  */
  .wrapper {
    &:hover .overlay {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
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
  }

  

  .card-body {
    z-index: 100;
    background-color: white;
  }

  .card-text {
    color: $primary;
  }
}
</style>