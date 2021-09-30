<template>
  <div id="app">
    <Header />
    <section id="slider"></section>
    <section id="gallery">
      <img src="./assets/img/h-2-port-img-1.jpg" alt="">
      <img src="./assets/img/h-2-port-img-2.jpg" alt="">
      <img src="./assets/img/h-2-port-img-3.jpg" alt="">
      <img src="./assets/img/h-2-port-img-4.jpg" alt="">
      <img src="./assets/img/h-2-port-img-5.jpg" alt="">
      <img src="./assets/img/h-2-port-img-6.jpg" alt="">
    </section>
    <section id="workingProcess"></section>
    <section id="workWithUs"></section>
    <section id="blog"></section>
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
@import '~@fortawesome/fontawesome-free/css/all.min.css';
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}

#gallery {
  display: flex;
  flex-wrap: wrap;
  img {
    width: calc(100% / 3);
  }
}
</style>
