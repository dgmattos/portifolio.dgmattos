<template>
  <nav class="navbar fixed-top navbar-expand-lg" :class="navclass">
    <div class="container-fluid">
      <a :class="brandClass" class="navbar-brand d-flex align-items-center text-fantasma" href="#inicio">
        <div class="icon-profile">
          <img src="src/assets/profile-2021.jpeg" alt="DEIVID G MATTOS">
        </div>
         <span class="text-fantasma ms-2">DEIVID G. MATTOS</span>
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
              aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <i class="fas fa-bars"></i>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#inicio">Início</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#sobre-mim">Sobre mim</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#formacao-academica">Formação acadêmica</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#formacao-tecnica">Formação Técnica</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#marcas-que-trabalhei">Marcas</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "navBarMenu",
  data: function () {
    return {
      pos: 0
    }
  },
  created: function(){
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed: function(){
    window.removeEventListener('scroll', this.handleScroll);
  },
  computed: {
    navclass: function () {
       if(this.pos <= 100){
        return "navbar-dark bg-dark hide-brand";
       }else{
         return "navbar-dark bg-dark shadow";
       }
    },
    brandClass: function () {
      if(this.pos <= 100){
        return "hide";
      }else{
        return "show";
      }
    }
  },
  methods: {
    handleScroll(event) {
      this.pos = window.pageYOffset;
    }
  }
}
</script>

<style scoped>
  .navbar{
    transition: 0.5s;
  }
</style>
