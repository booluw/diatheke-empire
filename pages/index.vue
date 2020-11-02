<template>
  <main>
    <app-jumbotron />
    <div class="placeholder"></div>
    <section class="section section--w-60">
      <h2 class="heading heading--sub">
        About Diatheke Empire
      </h2>
      <p class="paragraph">
        Diatheke Empire is a private owned investment company committed to better lives of populace and transform Africa.
      </p>
      <nuxt-link to="/about" class="section__link" title="Learn more about Diatheke Empire">Learn More</nuxt-link>
    </section>
    <section class="section">
      <h2 class="heading heading--sub">
        The Diatheke Empire Creed
      </h2>
      <div class="row row--mt2">
        <div class="col-2">
          <div class="card">
            <div class="card__big-text">E</div>
            <h3 class="card__heading">Excellence</h3>
            <p class="card__text">
              To be an exceptional company, where every product is at it's peak efficiency and provides it's maximum satisfaction.
            </p>
          </div>
        </div>
        <div class="col-2">
          <div class="card">
            <div class="card__big-text">I</div>
            <h3 class="card__heading">Integrity</h3>
            <p class="card__text">
              Upholding honesty and strong moral principles towards our investments and consumers to enhance stronger relationships.
            </p>
          </div>
        </div>
        <div class="col-2">
          <div class="card">
            <div class="card__big-text">I</div>
            <h3 class="card__heading">Innovation</h3>
            <p class="card__text">
              To create extraordinary products with a blend of creativity, modern ideas and new innovation that will standout among others.
            </p>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <h2 class="heading heading--sub">
        Our Investments
      </h2>
      <p class="paragraph paragraph--w-60">
        We invest in sectors that provide long term and short term solutions to Africa's problem, with
          adequate returns and have the ability to propel Africa's Economy forward.
      </p>
      <nuxt-link to="/investments" class="section__link" title="Learn more on Diatheke Empire investments.">Learn More</nuxt-link>
      <div class="row row--mt2">
        <div class="col-2">
          <nuxt-link to="/" class="card card--row">
            <img src="~/assets/img/favicon.png" class="card__img" alt="Diatheke Empire Logo" />
            <div class="card__body">
              <h3 class="card__heading">DLink</h3>
              <p class="card__paragraph">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam
              </p>
            </div>
          </nuxt-link>
        </div>
        <div class="col-2">
          <nuxt-link to="/" class="card card--row">
            <img src="~/assets/img/favicon.png" class="card__img" alt="Diatheke Empire Logo" />
            <div class="card__body">
              <h3 class="card__heading">DHH</h3>
              <p class="card__paragraph">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam
              </p>
            </div>
          </nuxt-link>
        </div>
        <div class="col-2">
          <nuxt-link to="/" class="card card--row">
            <img src="~/assets/img/favicon.png" class="card__img" alt="Diatheke Empire Logo" />
            <div class="card__body">
              <h3 class="card__heading">DCycler</h3>
              <p class="card__paragraph">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam
              </p>
            </div>
          </nuxt-link>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import AppJumbotronVue from '~/components/AppJumbotron.vue'


export default {
  name: 'HomePage',
  components: {
    'app-jumbotron': AppJumbotronVue
  },
  head() {
    return {
      title: 'Home || Diatheke Empire',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Diatheke Empire is a private owned investment company committed to better lives of populace and transform Africa.'
        },
        {
          property: 'og:title',
          content: 'Home || Diatheke Empire'
        },
        {
          property: 'og:description',
          content: 'Diatheke Empire is a private owned investment company committed to better lives of populace and transform Africa.'
        },
        {
          property: 'og:url',
          content: 'https://diathekeempire.com/'
        },
        {
          property: 'twitter:card',
          content: 'summary_large_image'
        }
      ]
    }
  }
}
</script>