<template>
  <nav class="navbar fixed-top navbar-expand-lg" :class="navclass">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
              aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Início</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Sobre mim</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Formação acadêmica</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Formação Técnica</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Marcas</a>
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
        return "navbar-dark bg-dark";
       }else{
         return "navbar-light bg-light shadow";
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
