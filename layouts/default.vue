<template>
  <div>
    <site-header />
    <Nuxt />
    <site-footer />
  </div>
</template>

<script>
import SiteHeader from '~/components/Header'
import SiteFooter from '~/components/Footer'

export default {
  components: {
    SiteHeader,
    SiteFooter
  }
}
</script>

<style lang="scss">
    @import "~/assets/scss/main.scss";
</style>
