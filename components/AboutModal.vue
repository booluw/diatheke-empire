<template>
  <section class="modal-container">
    <div class="modal">
      <button class="modal__btn ion icon ion-ios-close" @click="$emit('close')"></button>
      <div class="modal__body">
          <img :src="require(`~/assets/img/${data.img}.jpg`)" class="modal__img" :alt="`Photo of ${data.name}, ${data.title} Diatheke Empire`" />
          <div class="modal__content">
            <div class="__header">
              <h3 class="modal__heading">{{data.name}}</h3>
              <p>{{data.title}}</p>
          </div>
          <p class="modal__text" v-html="data.about"></p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AboutModal',
  props: {
    data: {
      required: true,
      type: Object
    }
  },
}
</script>

<style>

</style>