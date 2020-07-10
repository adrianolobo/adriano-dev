<template>
  <div id="app">
    <space />
  </div>
</template>

<script>
import Space from './components/space/space.vue';

export default {
  components: {
    Space,
  },
};
</script>

<style lang="sass">
  html, body
    width: 100%
    height: 100%
    font-family: 'Rubik', sans-serif
    font-size: calc(10px + 0.20vw)
  #app
    display: flex
    width: 100%
    height: 100%
  *
    box-sizing: border-box
</style>
