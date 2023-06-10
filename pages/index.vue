<template>
  <div>
    <div class="home-top-background bg-fran d-flex align-items-center justify-content-center">
        <div class="d-flex justify-content-center">
          <img src="~/assets/img/logo-sem-fundo.png" class="logo-img" alt="olivstudio">
    </div>
    </div>
    <div class="row m-0" id="sobre">
      <div class="col-lg-8 col-md-12 col-12 d-flex flex-column align-items-center justify-content-center">
        <h1 class="page-title">
        Oi!<br>
        Meu nome é Fran.<br>
        Sou fundadora e designer no Oliv.
        </h1>

        <h3 class="about-me mt-3">
          Formada em moda e há 11 anos atuando no mercado
          fashion e criativo, fundei o Oliv Studio com a missão
          de criar projetos visuais irreverentes, originais e com
          viés artístico. O estúdio conta com a colaboração
          de profissionais multidissiplinares, selecionados
          por perfil de acordo com cada projeto. Estas
          características refletem em criações singulares e
          repletas de personalidade, que encantam e atendem
          às necessidades do cliente, sem cair na obviedade.
        </h3>
      </div>

      <div class="col-lg-4 col-md-12 col-12 p-0">
        <img src="~/assets/img/sobre.png" class="w-100 sobre-fran-img" alt="olivstudio">
      </div>
    </div>

    <div class="bg-fran">
      <div class="container pt-5 pb-5">
        <span class="services-title">
          Conheça meus serviços!
        </span>
        <br>
        <span class="services-subtitle">
          Entenda um pouco sobre meus desenvolvimentos de
        </span>
        <div class="d-flex justify-content-between mt-3 white-list">
          <ul>
            <li>Identidade visual</li>
            <li>Criação de estampa</li>
            <li>Ilustração</li>
            <li>Projetos especiais</li>
          </ul>

          <div class="d-flex align-items-center">
          <b-button class="btn button-servicos" @click="redirectServicos()">
          Veja mais
          </b-button>
        </div>
        </div>
      </div>
    </div>

    <div class="mt-3 d-flex align-content-center align-items-center justify-content-center"> 
      <div class="carossel">
      <h1 class="text-center" style="color: rgb(185, 121, 214);">Ultimos projetos realizados:</h1>

        <VueSlickCarousel v-bind="slickOptions">
          <div>
            <img src="~/assets/img/projetos/gorgeous.png" class="carossel-img" alt="">
          </div>
          <div>
            <img src="~/assets/img/projetos/jumenezes.png" class="carossel-img" alt="">
          </div>
          <div>
            <img src="~/assets/img/projetos/optik.png" class="carossel-img" alt="">
          </div>
          <div>
            <img src="~/assets/img/projetos/smash.png" class="carossel-img" alt="">
          </div>
          <div>
            <img src="~/assets/img/projetos/yandara.png" class="carossel-img" alt="">
          </div>
        </VueSlickCarousel> 
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
        slidesToShow: 3,
        arrows: false,
        dots: false,
        infinite: true,
        speed: 600,
        centerMode: true,
        autoplay: true,
        responsive: [
          {
            breakpoint: 1024,
            settings: {
              slidesToShow: 1,
            },
          },
        ],
      }
    }
  },
  methods: {
    redirectServicos() {
      //inserir codigo analytics
      this.$router.push('/servicos')
    }
  }
}
</script>

<style scoped>
.page-title {
  font-size: 50px;
  color: rgb(185, 121, 214);
}

.about-me {
  width: 75%;
  font-weight: 300;
  font-size: 25px;
}
.carossel {
  height: 550px;
  width: 100%;
}

 .carossel-img {
  height: 500px;
  width: 500px;
  object-fit: cover;
}

.home-top-background {
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-position: center center;
  height: 650px;
}

.logo-img {
  height: 250px;
}


.button-servicos {
  height: 100px;
  width: 250px;
  background-color: transparent;
  color: white;
  border-color: white;
  font-size: 45px;
  font-weight: 300;
}

.services-title {
  font-size: 65px;
  color: white;
}

.services-subtitle {
  font-size: 25px;
  color: white;
}

.white-list ul li {
color: white;
font-size: 25px;
}

@media (max-width :767px) {
  .services-title {
  font-size: 35px;
}

.services-subtitle {
  font-size: 20px;
}

.white-list ul li {
font-size: 20px;
}

.button-servicos {
  height: 50px;
  width: 150px;
  font-size: 15px;
}

    .page-title {
    margin-top: 10px;
    font-size: 25px;
  }

  .about-me {
    width: 100%;
    font-size: 15px;
  }

  .sobre-fran-img {
    height: 385px;
    object-fit: cover;
  }
}
</style>

<style>
.bg-fran {
  background-color: #b8afce;
}
</style>
