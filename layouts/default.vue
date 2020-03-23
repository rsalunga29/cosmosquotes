<template>
  <div>
    <div class="flex justify-end">
      <nuxt-link class="mx-4 mb-4 md:my-3" to="/">Generate Quotes</nuxt-link>
      <nuxt-link class="mx-4 mb-4 md:my-3" to="/about">What is this?</nuxt-link>
    </div>

    <nuxt />

    <p class="text-white text-xs text-right mr-2 mb-2">
      <a href="https://www.vecteezy.com/free-vector/space">Space Vectors by Vecteezy</a>
    </p>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css?family=Kaushan+Script&display=swap');

html {
  background: url('~assets/img/bg.svg') no-repeat;
  background-position: center;
  background-size: cover;
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  @apply text-white;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.container {
  @apply min-h-screen flex justify-center items-center mx-auto;
}

.card {
  @apply flex flex-col justify-center rounded overflow-scroll shadow-lg bg-white text-black mb-6;
}

.card--quote {
  background: url('~assets/img/quotation-mark.svg'), #ffffff;
  background-repeat: no-repeat, no-repeat;
  background-size: 13%;
  background-position: top 0.775rem left 0.975rem, center;
  font-family: 'Kaushan+Script';
  height: 20rem;
  @apply text-lg tracking-widest;
}
</style>
