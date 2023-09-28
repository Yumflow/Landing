<template>
  <InlineSvg v-if="props.src.includes('.svg')" :src="props.src"></InlineSvg>
  <img v-else :src="props.src" :draggable="props.draggable" :alt="props.alt" />
</template>

<script setup lang="ts">
import InlineSvg from 'vue-inline-svg'

const props = defineProps({
  src: {
    type: String,
    required: true,
  },

  alt: {
    type: String,
  },

  draggable: {
    type: Boolean,
    default: true,
  },
})
</script>

<style lang="sass">
svg
  path:not([fill]),
  rect:not([fill]),
  g:not([fill]),
  ellipse:not([fill])
    fill: currentColor
</style>