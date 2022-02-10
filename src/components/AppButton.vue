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
  cursor: pointer;

  &.light {
    background-color: #fff;
    color: $primary;

    &:hover {
      background-color: $primary;
      color: #fff;
    }
  }

  &.dark {
    background-color: $primary;
    color: #fff;

    &:hover {
      background-color: $secondary;
      color: $primary;
    }
  }
}
</style>