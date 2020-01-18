<template>
  <header class="masthead">
    <div id="page-top" class="container d-flex h-100 align-items-center">
      <div class="mx-auto text-center">
        <carousel-3d>
          <slide :index="0">
            <img style="height: 100%" src="@/assets/pictures/hands.jpg" />
          </slide>
          <slide :index="1">
            <img src="@/assets/pictures/idea.jpg" />
          </slide>
          <slide :index="2">
            <img src="@/assets/pictures/hands.jpg" />
          </slide>
          <slide :index="3">
            <img src="@/assets/pictures/hands.jpg" />
          </slide>
        </carousel-3d>

        <h2 class="text-secondary-custom mx-auto mt-2 mb-5">
          {{ localsoustitre }}
        </h2>

        <a href="#about" class="btn btn-primary js-scroll-trigger"
          >En savoir plus</a
        >
      </div>
    </div>
  </header>
</template>

<script>
import { Carousel3d, Slide } from 'vue-carousel-3d'
import { state } from '../store/constantes'

export default {
  components: {
    Carousel3d,
    Slide
  },
  data() {
    return {
      localsoustitre: state().soustitre
    }
  }
}
</script>

<style scoped>
.masthead {
  position: relative;
  width: 100%;
  height: auto;
  min-height: 35rem;
  padding: 15rem 0;
  background: #badfdc;
  background-image: url('../assets/landscape/homme-voiture-blurred.jpg');
  /*background: linear-gradient(to bottom, rgba(22, 22, 22, 0.3) 0%, rgba(22, 22, 22, 0.7) 75%, #161616 100%), url("./punaise_banniere.jpeg");*/
  background-position: center;
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-size: cover;
}

img {
  height: 100%;
}

.masthead h1 {
  font-family: 'Berthold';
  font-size: 2.5rem;
  line-height: 2.5rem;
  letter-spacing: 0.8rem;
  background: -webkit-linear-gradient(
    rgba(255, 255, 255, 0.9),
    rgba(255, 255, 255, 0)
  );
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
}

.masthead h2 {
  max-width: 20rem;
  font-size: 1rem;
}

@media (min-width: 768px) {
  .masthead h1 {
    font-size: 4rem;
    line-height: 4rem;
  }
}

@media (min-width: 992px) {
  .masthead {
    height: 100vh;
    padding: 0;
  }
  .masthead h1 {
    font-size: 6.5rem;
    line-height: 6.5rem;
    letter-spacing: 0.8rem;
  }
  .masthead h2 {
    max-width: 30rem;
    font-size: 1.25rem;
  }
}
</style>
