<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  subtitle: {
    type: String,
    required: true
  },
  description: {
    type: String,
    required: true
  },
  imageUrl: {
    type: String,
    required: true
  },
  isReversed: {
    type: Boolean,
    required: false,
    default: false
  }
})
</script>

<template>
  <div class="wrapper">
    <div
      class="content justify-around flex-col-r-sm"
      :style="[isReversed ? { 'flex-direction': 'row-reverse' } : { 'flex-direction': 'row' }]"
    >
      <img :src="imageUrl" alt="Hero image" />
      <div class="text-wrapper flex flex-col gap-1">
        <h3>{{ title }}</h3>
        <h2>{{ subtitle }}</h2>
        <h4>{{ description }}</h4>
      </div>
    </div>
  </div>
</template>

<style scoped lang="sass">
@import 'src/assets/sass/variables.sass'
.wrapper
  padding: 1rem
  margin: 4rem 0
.content
  display: flex
  align-items: center
.text-wrapper
  max-width: 35.5rem
  @media (max-width: $layout-breakpoint-small)
    align-items: center
img
  width: 18.875rem
  height: 32.8125rem
  @media (max-width: $layout-breakpoint-small)
    margin-top: 2rem
</style>
