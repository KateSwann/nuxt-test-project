<template>
  <div>
    <Header />

    <nuxt/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import AppLogo from '@/components/AppLogo.vue'

export default {
  components: {
    Header,
    AppLogo
  }
}
</script>

<style>
</style>

