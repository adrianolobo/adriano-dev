<template>
  <div class="star" :style="starStyle"></div>
</template>

<script>
export default {
  props: {
    top: Number,
    left: Number,
  },
  computed: {
    starStyle() {
      return {
        top: `${this.top}%`,
        left: `${this.left}%`,
      };
    },
  },
};
</script>

<style lang="sass" scoped>

  .star
    width: 2px
    height: 2px
    background-color: #fff
    position: absolute
    border-radius: 50%
    left: 30%
    top: 30%
    transform: translate(-50%, -50%)

  .star:before
    content: ''
    position: absolute
    width: 40px
    height: 40px
    background: radial-gradient(circle, rgba(255,255,255,0.04) 0%, rgba(255,255,255,0) 80%)
    left: 50%
    top: 50%
    transform: translate(-50%, -50%)
</style>
