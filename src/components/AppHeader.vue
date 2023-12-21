<template>
  <header class="flex justify-between">
    <div class="logo-wrapper"><img class="logo-img" src="../assets/images/logo.png" /></div>
    <div class="gap-6 flex hide-sm">
      <a href="#" active>Home</a>
      <a href="#">Product</a>
      <a href="#">Faq</a>
      <a href="#">Contact</a>
    </div>
    <div class="hide-lg">
      <img src="../assets/icons/hamburger.svg" />
    </div>
  </header>
</template>

<style scoped lang="sass">
@import 'src/assets/sass/variables.sass'
.logo-wrapper
    display: flex
    @media (max-width: $layout-breakpoint-small)
        width: 100%
        height: 100%
.logo-img
    width: 12.875rem
    height: 6.35988rem
    flex-shrink: 0
    @media (max-width: $layout-breakpoint-small)
        width: 6.5rem
        height: 3rem

header
    display: flex
    align-items: center
    padding: 1.6rem 4.3rem
    @media (max-width: $layout-breakpoint-small)
        padding: 1rem 1rem
        height: 8rem
</style>
