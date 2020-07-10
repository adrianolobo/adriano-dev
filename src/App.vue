<template>
  <div id="app">
    <div class="space">
      <div class="space__stars">
        <div class="star star_1"></div>
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
  </div>
</template>

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
