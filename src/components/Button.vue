<template>
  <buttton :class="[{'btn__small': small},'btn']">
    <slot></slot>
  </buttton>
</template>

<script>
export default {
  props: {
    small: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style lang="scss">
  .btn {
    background-color: #2BDA53;
    color: white;
    padding: 1rem 3rem;
    border-radius: 3px;
    &__small {
      padding: 1rem 2rem;
    }
  }
</style>