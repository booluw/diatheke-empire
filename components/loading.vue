<template>
  <section class="loading" v-if="loading">
    <img src="~/assets/img/favicon.png" />
  </section>
</template>

<script>
export default {
  name: 'AppLoader',
  data() {
    return {
      loading: false
    }
  },
  methods: {
    start: function() {
      this.loading = true
    },
    finish: function () {
      this.loading = false
    }
  },
}
</script>

<style>

</style>