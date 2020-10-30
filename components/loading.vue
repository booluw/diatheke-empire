<template>
  <section class="loading" v-if="loading">
    <img src="~/assets/img/favicon.png" class="loading__img" />
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

<style scoped>
.loading {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-color: rgb(255, 255, 255);
  z-index: 10;

  display: flex;
  justify-content: center;
  align-items: center;
  transition: .3 ease-out;
}

.loading__img {
  width: 10rem;
  height: 10rem;
  animation-name: bounce;
  animation-timing-function: ease-out;
  animation-duration: 1s;
  animation-iteration-count: infinite;
}

@keyframes bounce {
  50% {
    transform: scale(.7);
  }
  70% {
    transform: scale(.9);
  }
  90% {
    transform: scale(1)
  }
  100% {
    transform: scale(.9)
  }
}
</style>