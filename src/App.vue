<template>
  <div id="app">
    <Header />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header"
import Footer from "./components/Footer"
export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}

</style>
