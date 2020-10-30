<template>
  <div>
    <header class="header">
      <input type="checkbox" id="toggle" style="display: none;" />
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
    <Nuxt />
  </div>
</template>