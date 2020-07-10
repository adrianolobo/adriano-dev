<template>
  <div class="space">
    <div class="space__stars">
      <star :top="33" :left="33"/>
      <star :top="50" :left="5"/>
      <star :top="70" :left="10"/>
      <star :top="70" :left="80"/>
      <star :top="25" :left="65"/>
      <star :top="7" :left="7"/>
    </div>
    <div class="space__text-container">
      <h1 class="space__hi">
        Hi.
      </h1>
      <p>
        My name is <strong>Adriano Lobo Lopes S. Dias</strong>
      </p>
      <p>
        I'm a <strong>front-end developer</strong>
        and I also love to create <strong>indie games</strong> in my free time.
      </p>
    </div>
  </div>
</template>

<script>
import Star from './star.vue';

export default {
  components: {
    Star,
  },
};
</script>

<style lang="sass" scoped>

  .space
    display: flex
    flex-direction: column
    height: 100%
    width: 100%
    justify-content: center
    align-items: center
    background-image: linear-gradient(to right bottom, #0e1d34, #192240, #26264b, #362a54, #472c5c)

  .space__stars
    width: 100%
    height: 100%
    position: absolute

  .space__hi
    font-size: 1.8em
    font-weight: 500
    margin-bottom: 1em

  .space__text-container
    font-size: 1.6em
    font-weight: 100
    color: #9c96bd
    width: 650px
    max-width: 100vw
    padding: 20px
</style>
