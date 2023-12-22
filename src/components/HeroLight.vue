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
  }
})
</script>

<template>
  <div class="content flex items-center justify-around flex-col-r-sm">
    <img :src="imageUrl" alt="Hero image" class="mt-2-sm" />
    <div class="text-wrapper flex flex-col gap-1 items-center-sm">
      <h3>{{ title }}</h3>
      <h2>{{ subtitle }}</h2>
      <h4>{{ description }}</h4>
    </div>
  </div>
</template>

<style scoped lang="sass">
@import 'src/assets/sass/variables.sass'
.content
  padding: 1rem
  margin: 4rem 0
.text-wrapper
  max-width: 35.5rem
</style>
