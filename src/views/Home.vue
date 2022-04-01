<template>
  <div>
    <nav-bar-menu />
      <section id="inico">
        <profile-pic src="src/assets/profile-2021.jpeg" alt=""></profile-pic>
      </section>
    <section id="academica">
      <academica></academica>
    </section>
    <section id="tecnica">
      <tecnica></tecnica>
    </section>
  </div>
</template>

<script>

import ProfilePic from "../components/profilePic.vue";
import navBarMenu from "../components/navBarMenu.vue";
import Tecnica from "../components/tecnica.vue";
import academica from "../components/tecnica.vue";
export default {
  name: "Home",
  components: {Tecnica, ProfilePic,navBarMenu,academica}

}
</script>

<style scoped>

</style>
