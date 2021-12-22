<template>
  <section>
    <app-jumbotron />
    <section class="section section--bg">
      <div class="row m-0 align-items-center justify-content-between">
        <div class="col-md-6 p-0">
          <h2 class="section__heading">
            About us
          </h2>
          <p class="section__paragraph">
            With operation starting in Nigeria, our investment portfolio includes leadership, clean energy and power, financial services, agriculture, transport and logistics, and education.
          </p>
          <nuxt-link to="/about-us" class="section__link">
            learn more
          </nuxt-link>
        </div>
      </div>
    </section>
  </section>
</template>

<script>
import AppJumbotron from '~/components/AppJumbotron.vue'
export default {
  components: { AppJumbotron },
  name: 'IndexPage'
}
</script>
