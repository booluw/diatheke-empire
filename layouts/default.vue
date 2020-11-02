<template>
  <div class="body">
    <header class="header" v-scroll="handleScroll" :class="{'header--fixed': scroll > 20}">
      <input type="checkbox" id="toggle" style="display: none;" ref="toggle"/>
      <nuxt-link to="/">
        <img src="~/assets/img/DIATHEKE-Empire-text-logo.png" class="header__logo" alt="DIATHEKE Empire text logo"/>
      </nuxt-link>
      <nav class="nav">
        <nuxt-link to="/about" class="nav__link" exact-active-class="nav__link--active">About</nuxt-link>
        <nuxt-link to="/contact" class="nav__link" exact-active-class="nav__link--active">Contact</nuxt-link>
        <nuxt-link to="/career" class="nav__link" exact-active-class="nav__link--active">Career</nuxt-link>
      </nav>
      <label class="header__hamburger" for="toggle">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
      </label>
    </header>
    <section class="social" :class="{'social--show': scroll > 100}">
      <a href="//facebook.com/diathekeempire" target="_blank" rel="noopener" class="social__link" title="Follow Diatheke Empire on Facebook">
        <i class="ion icon ion-logo-facebook"></i>
      </a>
      <a href="//twitter.com/diathekeempire" target="_blank" rel="noopener" class="social__link" title="Follow Diatheke Empire on Twitter">
        <i class="ion icon ion-logo-twitter"></i>
      </a>
      <a href="//linkedin.com/diathekeempire" target="_blank" rel="noopener" class="social__link" title="Connect with Diatheke Empire on Linkedin">
        <i class="ion icon ion-logo-linkedin"></i>
      </a>
      <a href="//instagram.com/diathekeempire" target="_blank" rel="noopener" class="social__link" title="Follow Diatheke Empire on Instagram">
        <i class="ion icon ion-logo-instagram"></i>
      </a>
    </section>
    <Nuxt />
  </div>
</template>
<script>
export default {
  name: 'AppLayout',
  data() {
    return {
      scroll: 0
    }
  },
  methods: {
    handleScroll: function() {
      this.scroll = window.scrollY
    },
    hideMenu: function() {
      this.$refs.toggle.checked = false
    },
  },
  watch: {
    '$route': function() {
      this.hideMenu()
    }
  },
  directives: {
    scroll: {
      inserted: function (el, binding) {
        let f = function (evt) {
          if (binding.value(evt, el)) {
            window.addEventListener('scroll', f)
          }
        }
        window.addEventListener('scroll', f)
      }
    }
  }
}
</script>