<template>
  <section id="academica">
    <div class="container animate__animated animate__fadeInUp">
      <h2 class="h2">
        Formação acadêmica
      </h2>
      <div class="row g3">
        <div class="col-12 p-3 col-sm-4  ms-auto me-auto animate__animated animate__fadeInUp" v-for="item in cursos">
          <div class="d-flex p-3  h-100 flex-column justify-content-center fant-border">
            <span class="fant" v-html="item.icon"></span>
            <span class="h4 mt-3  text-white text-fantasma">{{item.title}}</span>
            <small>{{item.description}}</small>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "academica",
  data: function () {
    return {
      cursos:[]
    }
  },
  mounted() {
    this.cursos.push({title: 'Análise e Desenvolvimento de sistemas', description: 'UCL - 2022', icon: '<i class="fas fa-award icon-fant"></i>'});

  }
}
</script>

<style scoped>

</style>
