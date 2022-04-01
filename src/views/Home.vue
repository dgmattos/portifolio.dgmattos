<template>
  <div>
    <nav-bar-menu />
    <topo></topo>
    <pessoal></pessoal>
    <academica></academica>
    <tecnica></tecnica>
    <marcas></marcas>
  </div>
</template>

<script>
import navBarMenu from "../components/navBarMenu.vue";
import Tecnica from "../components/tecnica.vue";
import academica from "../components/academica.vue";
import topo from "../components/topo.vue";
import pessoal from "../components/pessoal.vue";
import Marcas from "../components/marcas.vue";
export default {
  name: "Home",
  components: {Marcas, Tecnica,navBarMenu,academica,topo,pessoal},
  created() {

  }
}
</script>

<style scoped>

</style>

