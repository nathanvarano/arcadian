<script setup>
import HeroLight from './HeroLight.vue'
import AppHeader from './AppHeader.vue'
import AppFooter from './AppFooter.vue'
</script>

<template>
  <main>
    <app-header />
    <section>
      <div>
        <div class="header-banner-img w-full bg-light-sm absolute" />
      </div>
      <div class="header-banner w-full flex flex-col justify-end items-center relative">
        <div class="text-center flex flex-col gap-1 justify-end items-center w-full">
          <h3 class="text-light hide-sm">Food app</h3>
          <h5 class="hide-lg">Food app</h5>
          <h1 class="text-light hide-sm">Why stay hungry when you can order from Bella Onojie</h1>
          <h2 class="hide-lg">Why stay hungry when you can order from Bella Onojie</h2>
          <h4 class="text-light grey-text-sm">Download the Bella Onoje's food app now on</h4>
        </div>
        <div class="button-wrapper flex gap-1 justify-center flex-col-sm items-center">
          <button class="primary large">
            <a href="#" class="w-full h-full">
              <h3 class="text-light">Playstore</h3>
            </a>
          </button>
          <button class="secondary large border-accent-sm">
            <a href="#" class="w-full h-full">
              <h3 class="text-light text-accent-sm">App store</h3>
            </a>
          </button>
        </div>
      </div>
      <div class="flex justify-center" style="w-100%">
        <div class="phone-wrapper flex justify-center items-center">
          <img class="phones w-full z-2" src="../assets/images/phones.png" alt="" />
        </div>
      </div>
    </section>
    <div class="flex justify-center">
      <div id="how-the-app-works" class="flex justify-center">
        <h2>How the app works</h2>
      </div>
    </div>
    <section>
      <hero-light
        title="Create an account"
        subtitle="Create/login to an existing account to get started"
        description="An account is created with your email and a desired password"
        image-url="src/assets/images/phone-1.png"
      />
      <hero-light
        title="Explore varieties"
        subtitle="Shop for your favorites meal as e dey hot."
        description="Shop for your favorite meals or drinks and enjoy while doing it."
        image-url="src/assets/images/phone-2.png"
        class="flex-row-r"
      />
      <hero-light
        title="Checkout"
        subtitle="When you done check out and get it delivered."
        description="When you done check out and get it delivered with ease."
        image-url="src/assets/images/phone-3.png"
      />
    </section>
    <section>
      <div class="footer-banner flex flex-col justify-center items-center bg-dark-sm">
        <div class="text-wrapper flex flex-col justify-center items-center gap-1">
          <h2 class="text-light">Download the app now.</h2>
          <div>
            <h4 class="text-light hide-sm">
              Available on your favorite store. Start your premium experience now
            </h4>
            <h4 class="text-light hide-lg">Most calendars are designed for teams.</h4>
          </div>
        </div>
        <div class="button-wrapper flex gap-1 justify-center">
          <button class="primary small"><a href="#" class="text-light">Playstore</a></button>
          <button class="secondary small hide-sm">
            <a href="#" class="text-light h-full w-full">App store</a>
          </button>
          <button class="secondary small hide-lg">
            <a href="#" class="text-light h-full w-full">Try for free</a>
          </button>
        </div>
      </div>
    </section>
    <app-footer />
  </main>
</template>

<style scoped lang="sass">
@import 'src/assets/sass/variables.sass'
.header-banner
  height: clamp(31rem, $layout-breakpoint-small, 29rem)

.button-wrapper
  margin-top: 2.5rem

.header-banner-img
  height: 39rem
  background: $banner-gradient, url(src/assets/images/header-banner.jpeg) center / cover

.footer-banner
  height: 32rem
  background: $banner-gradient, url(src/assets/images/footer-banner.jpeg) center / cover

.phone-wrapper
  padding-bottom: 8rem

#how-the-app-works
  max-width: 55rem
  @media (min-width: $layout-breakpoint-small)
    border-top: 0.2rem solid #e4e4e4
    padding-top: 4rem
  @media (max-width: $layout-breakpoint-small)
    padding-bottom: 4rem !important
    border-bottom: 0.2rem solid #e4e4e4
    > h2
      font-size: 1.5rem !important
</style>
