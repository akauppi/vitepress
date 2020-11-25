<template>
  <div class="home">
    <HomeHero />
    <slot name="hero" />
    <HomeFeatures />
    <slot name="features" />
    <HomeFooter />
    <slot name="footer" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HomeHero from './HomeHero.vue'
import HomeFeatures from './HomeFeatures.vue'
import HomeFooter from './HomeFooter.vue'

export default defineComponent({
  components: {
    HomeHero,
    HomeFeatures,
    HomeFooter
  }
})
</script>
