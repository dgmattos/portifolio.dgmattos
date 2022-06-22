<template>
  <section id="marcas-que-trabalhei" class="bg-fantasma">
    <div class="container">
      <h2 class="h2">
        Marcas que já atuei
      </h2>
      <hr class="tt-bar">
      <div class="bg-ligh p-3">
        <carousel :items-to-show="itensShow" :autoplay="1500" :wrapAround="true">
          <slide v-for="item in logos" :key="item">
            <img class="logos-clientes" :src="item.src" :alt="item.label">
          </slide>
        </carousel>
      </div>
    </div>
  </section>
</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';

export default {
  name: "marcas",
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  created() {
    this.logos.push({label:'acalanto',src:'https://dgmattos.com.br/clientes/acalanto-300x169-1.png',lft:0});
    this.logos.push({label:'betha_espaco',src:'https://dgmattos.com.br/clientes/betha_espaco-300x169-1.png',lft:0});
    this.logos.push({label:'brincaqui',src:'https://dgmattos.com.br/clientes/brincaqui_site_300x157-2.png',lft:0});
    this.logos.push({label:'liga-de-mkt',src:'https://dgmattos.com.br/clientes/liga-de-mkt-logo-1.png',lft:0});
    this.logos.push({label:'abeps',src:'https://dgmattos.com.br/clientes/logo-abeps-1.png',lft:0});
    this.logos.push({label:'arcelormittal',src:'https://dgmattos.com.br/clientes/logo-arcelormittal.png',lft:0});
    this.logos.push({label:'banestes',src:'https://dgmattos.com.br/clientes/logo-banestes.png',lft:0});
    this.logos.push({label:'causeiobem',src:'https://dgmattos.com.br/clientes/logo-causeiobem-1.png',lft:0});
    this.logos.push({label:'conclua',src:'https://dgmattos.com.br/clientes/logo-conclua.png',lft:0});
    this.logos.push({label:'gava',src:'https://dgmattos.com.br/clientes/logo-gava-cred-imob.png',lft:0});
    this.logos.push({label:'klinger_publicidade',src:'https://dgmattos.com.br/clientes/logo-klinger_publicidade-1.png',lft:0});
    this.logos.push({label:'Lara-Machado',src:'https://dgmattos.com.br/clientes/Logo-Lara-Machado.png',lft:0});
    this.logos.push({label:'oncovit',src:'https://dgmattos.com.br/clientes/logo-oncovit.png',lft:0});
    this.logos.push({label:'premio-mulher',src:'https://dgmattos.com.br/clientes/logo-premio-mulher-1.png',lft:0});
    this.logos.push({label:'promoves',src:'https://dgmattos.com.br/clientes/logo-promoves-1.png'});
    this.logos.push({label:'roda-de-buteco',src:'https://dgmattos.com.br/clientes/logo-roda-de-buteco.png',lft:0});
    this.logos.push({label:'trovao-dos-mares',src:'https://dgmattos.com.br/clientes/logo-trovao-dos-mares-azul-1.png',lft:0});
    this.logos.push({label:'aluga_facil',src:'https://dgmattos.com.br/clientes/logo_aluga_facil-300x169-1.png',lft:0});
    this.logos.push({label:'sollo',src:'https://dgmattos.com.br/clientes/sollo-logo-1.png',lft:0});
    this.logos.push({label:'wtyt',src:'https://dgmattos.com.br/clientes/wtyt-300x169-1.png',lft:0});


  },
  mounted() {
    //this.rodar();
    let width = window.innerWidth;

    if (width <= 400){
      this.itensShow = 2;
    }else{
      this.itensShow = 6;
    }
  },
  data:function(){
    return {
      itensShow:4,
      logos:[],
      roda:'',
      lft:0,
    }
  },
  methods:{
    rodar:function(){
     /*
      let axu ='';
      let self = this;
      setInterval(function(){
        axu = self.logos[0];
        self.logos.push(axu);
        self.logos.shift();
      },1000);
     * */
    }
  }


}
</script>

<style scoped>
  .logos-clientes{
    display: flex;
    overflow: hidden !important;
  }
   img.logos-clientes{
    max-width: 150px;
    transition: 0.5s;
  }
  .carol{
    transition: 0.5s;
  }
  .bg-ligh{
    background-color:#fff !important;
  }
</style>
