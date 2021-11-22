<template>
  <div id="app">
    <Head></Head>
    <Main></Main>
  </div>
</template>

<script>
import Head from './components/Header.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Head,
    Main
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";

</style>
