<template>
  <button :class="[{'btn__small': small},'btn']">
    <slot></slot>
  </button>
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
    padding: 1rem 4rem;
    border-radius: 3px;
    border: 1px solid #2BDA53;
    &__small {
      padding: 1rem 2rem;
    }
  }
</style>