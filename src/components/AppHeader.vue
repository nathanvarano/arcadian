<template>
  <header class="flex justify-between">
    <img class="logo-img" src="../assets/images/logo.png" />
    <div class="gap-6 flex hide-sm items-center">
      <a href="#" active>Home</a>
      <a href="#">Product</a>
      <a href="#">Faq</a>
      <a href="#">Contact</a>
    </div>
    <div class="hide-lg flex items-center">
      <img src="../assets/icons/hamburger.svg" />
    </div>
  </header>
</template>

<style scoped lang="sass">
@import 'src/assets/sass/variables.sass'
.logo-img
    width: 12.9rem
    height: 6.3rem
    @media (max-width: $layout-breakpoint-small)
        width: 6.5rem
        height: 3rem

header
    padding: 1.6rem 4.3rem
    @media (max-width: $layout-breakpoint-small)
        padding: 1rem 1rem
        height: 6rem
</style>
