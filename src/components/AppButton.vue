<template>
  <div class="button" :class="theme">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    theme: String,
  }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.button {
  display: inline-block;
  font-size: .8rem;
  padding: 1em 2em;
  border-radius: 5px;

  &.light {
    background-color: #fff;
    color: $primary;
  }
  &.dark {
    background-color: $primary;
    color: #fff;
  }
}
</style>