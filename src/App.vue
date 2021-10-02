<template>
  <div id="app">
    <Header />
    <section id="slider">
      <div class="arrow left">
        <i class="fas fa-chevron-left"></i>
      </div>
      <div class="container">
        <div class="left">
          <h1>Devotion that never <span class="lobster-font">ends</span></h1>
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
    <section id="workingProcess">
      <div class="container">
        <h1>Working <span class="lobster-font">process</span></h1>
        <div class="wrapper">
          <img src="./assets/svg/svg-3.svg" alt="">
          <div class="card">
            <div class="circle">
              <i class="far fa-lightbulb"></i>
            </div>
            <div class="text">
              <h4>First there is an idea</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
          </div>
          <div class="card">
            <div class="circle">
              <i class="far fa-comment"></i>
            </div>
            <div class="text">
              <h4>Then we talk about</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
          </div>
          <div class="card">
            <div class="circle">
              <i class="fas fa-cloud"></i>
            </div>
            <div class="text">
              <h4>And we think about</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
          </div>
          <div class="card">
            <div class="circle">
              <i class="fas fa-pencil-alt"></i>
            </div>
            <div class="text">
              <h4>So we draw along</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="workWithUs">
      <h1>want to work with us? Send us <span class="lobster-font">a message!</span></h1>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maxime, quae eaque veritatis enim reprehenderit reiciendis doloremque molestias corrupti sed beatae. Earum qui adipisci voluptas natus, laboriosam asperiores aut deserunt nemo!</p>
      <div class="button">CONTACT</div>
    </section>
    <section id="blog">
      <div class="container">
        <div class="card">
          <img src="./assets/img/h-2-blog-img-1.jpg" alt="">
          <h4>This way, loves: a detailed guide through new design</h4>
          <p class="lobster-font">By Emily Fields</p>
        </div>
        <div class="card">
          <img src="./assets/img/h-2-blog-img-2.jpg" alt="">
          <h4>I try to give people a different way of looking art</h4>
          <p class="lobster-font">By Emily Fields</p>
        </div><div class="card">
          <img src="./assets/img/h-2-blog-img-3.jpg" alt="">
          <h4>Introduce Richard Laperrière of those amazing features</h4>
          <p class="lobster-font">By Emily Fields</p>
        </div>
      </div>
    </section>
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
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}
.lobster-font {
  font-family: 'Lobster', cursive;
}
.container {
  width: 60%;
  margin: auto;
}
p {
  font-size: 12px;
  line-height: 25px;
  color: gray;
}

#slider {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 70px 0;
  .container {
    display: flex;
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

#workingProcess {
  .container {
    width: 60%;
    margin: auto;
    text-align: center;
    padding: 50px 0;
    h1 {
      font-size: 60px;
      font-weight: 300;
      margin-bottom: 20px;
    }
    .wrapper {
      position: relative;
      display: flex;
      flex-wrap: wrap;
      img {
        position: absolute;
        top: 0;
        left: 50%;
        transform: translate(-50%);
        z-index: -1;
        width: 80%;
      }
      .card {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: calc(100% / 4);
        padding: 10px;
        .circle {
          display: flex;
          justify-content: center;
          align-items: center;
          height: 100px;
          width: 100px;
          border-radius: 50%;
          margin-bottom: 20px;
          background-color: #FAF7F1;
          i {
            font-size: 40px;
          }
          .fa-lightbulb {
            color: #C0E1CF;
          }
          .fa-cloud {
            color: #80465F;
          }
          .fa-comment {
            color: #F8D12D;
          }
          .fa-pencil-alt {
            color: #EB6950;
          }
        }
        .text {
          h4 {
            margin-bottom: 10px;
          }
        }
      }
    }
  }
}

#workWithUs {
  padding: 100px 250px;
  background-image: url(./assets/img/h-2-background-1.jpg);
  background-size: cover;
  background-position: center;
  text-align: center;
  h1 {
    font-size: 50px;
    font-weight: 300;
    padding-top: 20px;
    margin-bottom: 20px;
  }
  p { 
    margin-bottom: 30px;
  }
  .button {
    display: inline-block;
    font-size: 11px;
    font-weight: 600;
    padding: 10px 20px;
    background-color: #C0E1CF;
  }
}

#blog {
  .container {
    display: flex;
    padding: 70px 0;
    .card {
      display: flex;
      flex-direction: column;
      width: calc(100% / 3);
      padding: 10px;
      img {
        width: 100%;
        margin-bottom: 20px;
      }
      h4 {
        line-height: 25px;
      }
    }
  }
}
</style>
