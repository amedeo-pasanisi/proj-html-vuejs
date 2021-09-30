<template>
  <div id="app">
    <Header />
    <section id="slider">
      <div class="arrow left">
        <i class="fas fa-chevron-left"></i>
      </div>
      <div class="container">
        <div class="left">
          <h1>Devotion that never ends</h1>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Iure eligendi, deleniti aspernatur adipisci quibusdam et assumenda porro</p>
          <div class="button">READ MORE</div>
        </div>
        <div class="right">
          <img src="./assets/img/h-2-slider-img-15.png" alt="">
          <img src="./assets/img/h-2-slider-img-16.png" alt="">
        </div>
      </div>
      <div class="dots">
        <i class="fas fa-circle"></i>
        <i class="fas fa-circle"></i>
        <i class="fas fa-circle"></i>
      </div>
      <div class="arrow right">
        <i class="fas fa-chevron-right"></i>
      </div>
    </section>
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

#slider {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 70px 0;
  .container {
    display: flex;
    width: 60%;
    margin: auto;
    .left {
      width: 50%;
      h1 {
        font-size: 65px;
        font-weight: 300;
        margin-bottom: 20px;
      }
      p {
        font-size: 13px;
        margin-bottom: 20px;
        color: gray;
      }
      .button {
        display: inline-block;
        font-size: 11px;
        font-weight: 600;
        padding: 10px 20px;
        border: 2px solid #F3D0C7;
      }
    }
    .right {
      width: 50%;
      display: flex;
      img {
        height: 300px;
      }
    }
  }
  .arrow {
    position: absolute;
    height: 25px;
    width: 25px;
    border-radius: 50%;
    color: white;
    background-color: #F3D0C7;
    &.left {
      left: 20px;
    }
    &.right {
      right: 20px;
    }
    i {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
  .dots {
    position: absolute;
    bottom: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 60px;
    color: #F3D0C7;
    font-size: 6px;
    i:last-child {
      font-size: 7px;
    }
  }
}

#gallery {
  display: flex;
  flex-wrap: wrap;
  img {
    width: calc(100% / 3);
  }
}
</style>
