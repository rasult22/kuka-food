<template>
  <svg slot="icon" :class="`ic-${size} ic-${fill}`" >
    <use :xlink:href="require('@/assets/sprite.svg') + `#${icon}`" />
  </svg>
</template>

<script>
export default {
  props: {
    icon: {
      default: () => 'heart-circle'
    },
    size: {
      default: () => 16
    },
    fill: {
      default: () => 'primary'
    }
  }
}
</script>

<style>

</style>