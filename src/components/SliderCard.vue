<template>
  <div class="card">
    <img class="card-img-top" :src="`/images/${items[index].url}.jpg`" alt="product">
    <div v-if="withText" class="card-body text-center">
      <h6 class="card-title">{{ items[index].name }}</h6>
      <div class="card-text">{{ items[index].price }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    items: Array,
    withText: Boolean,
    index: Number,
  }
}
</script>

<style lang="scss" scoped>

</style>