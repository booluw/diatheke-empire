<template>
  <section>
    <app-header />
    <nuxt-child />
  </section>
</template>

<script>
import AppHeader from '~/components/AppHeader.vue'
export default {
  components: { AppHeader },

}
</script>
