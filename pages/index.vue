<template>
  <div>
    <div class="home-top-background d-flex align-items-center justify-content-center">
      <div class="container">
        <div class="d-flex justify-content-between">
          <img src="~/assets/img/logo-sem-fundo.png" class="logo-img" alt="olivstudio">
          <div class="carossel">
            <span>Ultimos clientes:</span>
            <VueSlickCarousel v-bind="slickOptions">
              <div>
                <img src="~/assets/img/clientes/fernandanasses.png" class="carossel-img" alt="">
              </div>
              <div>
                <img src="~/assets/img/clientes/jmenezes.png" class="carossel-img" alt="">
              </div>
              <div>
                <img src="~/assets/img/clientes/yume.png" class="carossel-img" alt="">
              </div>
            </VueSlickCarousel>
          </div>
        </div>
        <h1>Crie uma nova cara para sua marca</h1>
        <div class="w-100 d-flex justify-content-center">
          <b-button class="btn button-contratar mt-5" @click="redirectContrate()">
            Saiba como
          </b-button>
        </div>
      </div>
    </div>
    <div class="container ">
      <div class="text-center">
        <p style="font-size: 40px;">
          Por que você precisa de mim?
        </p>
        <p>
          Bom eu tenho otimas qualidades
        </p>
        <p>
          Bom eu tenho otimas qualidades
        </p>
        <p>
          Bom eu tenho otimas qualidades
        </p>
      </div>

      <div class="mt-4">
        <h5>AWDAWDAW</h5>
        <span>Opinião dos clientes:</span>
      </div>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'

export default {
  name: 'IndexPage',
  components: { VueSlickCarousel },
  data() {
    return {
      slickOptions: {
        slidesToShow: 1,
        arrows: false,
        dots: false,
        infinite: true,
        speed: 600,
        autoplay: true
      }
    }
  },
  methods: {
    redirectContrate() {
      //inserir codigo analytics
      this.$router.push('/contrate')
    }
  }
}
</script>

<style scoped>
.carossel {
  height: 280px;
  width: 50%;
}

.carossel-img {
  height: 250px;
  width: 250px;
  object-fit: cover;
}

.home-top-background {
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-position: center center;
  background-image: url(~/assets/img/background.jpg);
  height: 550px;
}

.logo-img {
  height: 250px;
}

h1 {
  color: rgb(255, 255, 255);
  font-weight: 700;
  text-shadow: 0.3px 0.5px 0.2px #000000;
}

.button-contratar {
  height: 60px;
  width: 200px;
  background-color: white;
  color: black
}
</style>
