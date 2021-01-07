<template>
  <div>
    <Nav />
    <section>
      <div class="main row">
        <Nuxt />
      </div>
    </section>
  </div>
</template>

<script>
import Nav from './partials/nav';
export default {
  components: {
    Nav
  }
}
</script>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
.main {
  max-width: 1000px;
  width: 80%;
  margin: auto;
}
.row {
  padding: 6% 0;
}
h1 {
  font-weight: normal;
    text-transform: uppercase;
    letter-spacing: 0.1em;
}
</style>
