<template>
  <div>
    <nav-bar-menu />
    <topo></topo>
    <wave class="bg-fantasma"/>
    <pessoal></pessoal>
    <wave fill="#939da7"/>
    <academica></academica>
    <tecnica></tecnica>
    <wave class="bg-fantasma"/>
    <marcas></marcas>
    <footerCopyRight></footerCopyRight>
  </div>
</template>

<script>
import navBarMenu from "../components/navBarMenu.vue";
import Tecnica from "../components/tecnica.vue";
import academica from "../components/academica.vue";
import topo from "../components/topo.vue";
import pessoal from "../components/pessoal.vue";
import Marcas from "../components/marcas.vue";
import Wave from "../components/wave.vue";
import footerCopyRight from "../components/footerCopyRight.vue";
export default {
  name: "Home",
  components: {Wave, Marcas, Tecnica,navBarMenu,academica,topo,pessoal,footerCopyRight},
  created() {

  }
}
</script>

<style scoped>

</style>

