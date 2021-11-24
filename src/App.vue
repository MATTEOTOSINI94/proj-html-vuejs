<template>
  <div id="app">
    <Head></Head>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Head from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Head,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "~font-awesome/css/font-awesome.css";
</style>
