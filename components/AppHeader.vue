<template>
  <header class="header">
    <input type="checkbox" name="hamburger__toggler" id="hamburger__toggler" class="hamburger__toggler" />
    <nuxt-link to="/" class="header__logo">
      <img src="~/assets/img/DIATHEKE-Empire-text.png" class="header__logo" />
    </nuxt-link>
    <nav class="header__nav">
      <ul class="nav">
        <li class="nav__dropdown">
          <nuxt-link to="/about-us" class="nav__link">
            About us
            <i class="lni lni-chevron-right"></i>
          </nuxt-link>
          <div class="nav__dropdown-container">
            <nuxt-link to="/about-us" class="nav__dropdown-link">Overview</nuxt-link>
            <nuxt-link to="/about-us#history" class="nav__dropdown-link">History</nuxt-link>
            <nuxt-link to="/about-us#leadership" class="nav__dropdown-link">Leadership</nuxt-link>
          </div>
        </li>
        <li class="nav__dropdown">
          <nuxt-link to="/investment" class="nav__link">
            Investment
            <i class="lni lni-chevron-right"></i>
          </nuxt-link>
          <div class="nav__dropdown-container">
            <nuxt-link to="/investment" class="nav__dropdown-link">Overview</nuxt-link>
            <nuxt-link to="/investment#agriculture" class="nav__dropdown-link">agriculture</nuxt-link>
            <nuxt-link to="/investment#education" class="nav__dropdown-link">education</nuxt-link>
            <nuxt-link to="/investment#energy" class="nav__dropdown-link">energy</nuxt-link>
            <nuxt-link to="/investment#finance" class="nav__dropdown-link">finance</nuxt-link>
            <nuxt-link to="/investment#transport" class="nav__dropdown-link">transport</nuxt-link>
          </div>
        </li>
        <li class="nav__dropdown">
          <nuxt-link to="/career" class="nav__link">
            career
            <i class="lni lni-chevron-right"></i>
          </nuxt-link>
          <div class="nav__dropdown-container">
            <nuxt-link to="/career" class="nav__dropdown-link">Overview</nuxt-link>
            <nuxt-link to="/career#work-culture" class="nav__dropdown-link">work culture</nuxt-link>
            <nuxt-link to="/career#work-at-diatheke" class="nav__dropdown-link">work at diatheke</nuxt-link>
          </div>
        </li>
        <li>
          <nuxt-link to="/philanthropy" class="nav__link">
            Philanthropy
            <i class="lni lni-chevron-right"></i>
          </nuxt-link>
        </li>
      </ul>
    </nav>
    <label for="hamburger__toggler" class="hamburger">
      <div class="hamburger__line"></div>
      <div class="hamburger__line"></div>
      <div class="hamburger__line"></div>
    </label>
  </header>
</template>

<script>
export default {
  name: 'AppHeader'
}
</script>
