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
    <section class="section">
      <h2 class="section__heading">
        investment profile
      </h2>
      <div class="row m-0 justify-content-between">
        <div class="col-md-6 p-0">
          <p class="section__paragraph">
            The ideology of Africapitalism by our role model Tony Elumelu, CON which is the private sector's commitment to Africa's development through long-term investments that build economic prosperity and social richness, guides our investing approach.
          </p>
          <nuxt-link to="/investment" class="section__link">
            learn more
          </nuxt-link>
        </div>
      </div>
      <br /><br />
      <div class="row m-0 justify-content-start align-items-center">
        <div class="col-md-3 p-0">
          <nuxt-link to="/investment#agriculture" class="card card--gradient">
            <img src="~/assets/img/agricultural-sector.jpg" class="card__img" />
            <div class="card__body">
              Agriculture
            </div>
          </nuxt-link>
        </div>
        <div class="col-md-3 p-0">
          <nuxt-link to="/investment#education" class="card card--gradient">
            <img src="~/assets/img/education.jpg" class="card__img" /><div class="card__body">
              Education
            </div>
          </nuxt-link>
        </div>
        <div class="col-md-3 p-0">
          <nuxt-link to="/investment#energy" class="card card--gradient">
            <img src="~/assets/img/energy-sector.jpg" class="card__img" />
            <div class="card__body">
              Energy
            </div>
          </nuxt-link>
        </div>
        <div class="col-md-3 p-0">
          <nuxt-link to="/investment#transport" class="card card--gradient">
            <img src="~/assets/img/transportation.jpg" class="card__img" /><div class="card__body">
              Transportation
            </div>
          </nuxt-link>
        </div>
      </div>
    </section>
    <section class="section section--no-padding section--bg">
      <div class="row align-items-center justify-content-between">
        <div class="col-md-6 p-0">
          <img src="~/assets/img/LUE.jpg" class="section__img section__img--padded" />
        </div>
        <div class="col-md-6 p-0">
          <h2 class="section__heading">Our Initiatives</h2>
          <p class="section__paragraph">
            Entrepreneurship isn't just about starting a business or leading an enterprise, we believe it is a skill-set and way of thinking that drives creativity and innovation. Its core is about building solutions to problems and taking the right steps to make them a reality. Entrepreneurs are not just business owners but passionate problem solvers
          </p>
          <nuxt-link to="/initiative" class="section__link">
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
