<template>
  <main>
    <about-jumbotron />    
    <div class="placeholder"></div>
    <section class="section section--w-60">
      <h2 class="heading heading--sub">
        Mission
      </h2>
      <p class="paragraph">
        Diatheke is committed to improving livelihood, through regeneration of capital and distribution of resources for a stable economy.
      </p>
    </section>    
    <section class="section section--w-60">
      <h2 class="heading heading--sub">
        Vision
      </h2>
      <p class="paragraph">
        To be a leading company towards improving the economy of the nation, empowering her citizens to ensure a sustainable living and maintain inter and intra organizational relationship.
      </p>
    </section>
    <section class="section">
      <h2 class="heading heading--sub">Executive Team</h2>
      <div class="row row--justify-spaced row--mt2">
        <div class="col-2" v-for="(person, index) in excos" :key="index" @click="modal = person">
          <div class="card card--exco">
            <img :src="require(`~/assets/img/${person.img}.jpg`)" class="card__img" :alt="`Photo of ${person.name}, ${person.title} Diatheke Empire`" />
            <div class="card__body">
              <h3 class="card__heading">{{person.name}}</h3>
              <p class="card__paragraph">{{person.title}}</p>
            </div>
          </div>
        </div>
      </div>
      <div class="row row--justify-spaced row--mt2">
        <div class="col-2" v-for="(person, index) in excos_2" :key="index" @click="modal = person">
          <div class="card card--exco">
            <img :src="require(`~/assets/img/${person.img}.jpg`)" class="card__img" :alt="`Photo of ${person.name}, ${person.title} Diatheke Empire`" />
            <div class="card__body">
              <h3 class="card__heading">{{person.name}}</h3>
              <p class="card__paragraph">{{person.title}}</p>
            </div>
          </div>
        </div>
      </div>
      <div class="row row--justify-center row--mt2">
        <div class="col-2"></div>
        <div class="col-2" v-for="(person, index) in excos_3" :key="index" @click="modal = person">
          <div class="card card--exco">
            <img :src="require(`~/assets/img/${person.img}.jpg`)" class="card__img" :alt="`Photo of ${person.name}, ${person.title} Diatheke Empire`" />
            <div class="card__body">
              <h3 class="card__heading">{{person.name}}</h3>
              <p class="card__paragraph">{{person.title}}</p>
            </div>
          </div>
        </div>
        <div class="col-2"></div>
      </div>
    </section>
    <about-modal v-if="modal" :data="modal" @close="modal = null" />
  </main>
</template>

<script>
import AboutJumbotronVue from '~/components/AboutJumbotron.vue'
import AboutModalVue from '~/components/AboutModal.vue'

export default {
  components: {
    'about-jumbotron': AboutJumbotronVue,
    'about-modal': AboutModalVue
  },
  data() {
    return {
      modal: null,
      excos: [
        {
          name: 'David Utulor',
          title: 'CEO',
          img: 'David-Utulor',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
        {
          name: 'Eric Limoh',
          title: 'COO',
          img: 'Limoh',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
        {
          name: 'Ebune Emmanuel',
          title: 'CFO',
          img: 'Ebune',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
        {
          name: 'Samuel Yusuf',
          title: 'CIO',
          img: 'Yusuf',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        }
      ],
      excos_2: [
        {
          name: 'Paul Bala',
          title: 'CPO',
          img: 'David-Utulor',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
        {
          name: 'Ejiofor Able',
          title: 'CHRO',
          img: 'David-Utulor',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
        {
          name: 'Paul Agih',
          title: 'VP Marketing',
          img: 'David-Utulor',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
        {
          name: 'Jessica Zynab Nagya',
          title: 'Quality Manager',
          img: 'David-Utulor',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        }
      ],
      excos_3: [
        {
          name: 'Given Ehi Owoicho',
          title: 'Accountant',
          img: 'Yusuf',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
        {
          name: 'Mercy Isah',
          title: 'Office Manager',
          img: 'Yusuf',
          about: `
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime omnis earum minus voluptatem quidem distinctio. Ex aliquid culpa harum fuga, excepturi tempore esse neque dicta doloribus dignissimos iure sapiente ea.
          `
        },
      ]
    }
  },
  head() {
    return {
      title: 'About Us || Diatheke Empire',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'About Diatheke: Diatheke is committed to improving livelihood, through regeneration of capital and distribution of resources for a stable economy.'
        },
        {
          property: 'og:title',
          content: 'About Us || Diatheke Empire'
        },
        {
          property: 'og:description',
          content: 'About Diatheke: Diatheke is committed to improving livelihood, through regeneration of capital and distribution of resources for a stable economy.'
        },
        {
          property: 'og:url',
          content: 'https://diathekeempire.com/about'
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