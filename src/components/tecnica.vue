<template>
  <section id="formacao-tecnica">
    <div class="container animate__animated animate__fadeInUp">
      <h2 class="h2">
        Formação Técnica recente
      </h2>
      <hr class="tt-bar">
      <div class="row g3">
        <div class="col-12 p-3 col-sm-3  ms-auto me-auto animate__animated animate__fadeInUp" v-for="item in cursos">
          <div class="d-flex p-3 h-100 flex-column justify-content-center fant-border">
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
  name: "tecnica",
  data: function () {
    return {
      cursos:[]
    }
  },
  mounted() {
    this.cursos.push({title: 'LGPD - Política de privacdiade', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'LGPD - Aplicada', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'LGPD - Fundamentos', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'PCI - (Payment Card) Standards for Corporate Professionals', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'Secure Programming Foundation', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'Modelagem Ágil de Processos', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'Dev. IOS 11 Swift 4', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'Material desing for android', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'VUE - Fundamentos', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'VUE - Criação de interfaces', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'Asp.net Core 2, Angular + EF Core', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'Angular fundamentos', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'C# (C Sharp) - ADO.NET', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});
    this.cursos.push({title: 'C# (C Sharp) - Entity e LINQ Framework', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});



    this.cursos.push({title: 'Criação de sites com Wordpress', description: '', icon: '<i class="fas fa-award icon-fant"></i>'});


  }
}
</script>

<style scoped>

</style>
