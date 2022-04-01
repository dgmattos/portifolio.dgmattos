<template>
  <section id="inicio">
    <div>
      <div class="profile-frame  animate__animated animate__fadeInUp" :style="{backgroundImage:'url(' + src + ')'}">
      </div>
      <h1 class="h1 text-white mt-3 animate__animated animate__fadeInUp">DEIVID GUSTAVO MATTOS</h1>
      <social-buttons class="animate__animated animate__fadeInUp" />
    </div>
  </section>
</template>

<script>
import socialButtons from "./socialButtons.vue";
export default {
  name: "topo",
  components: {socialButtons},

  data:function(){
    return {
      src:'src/assets/profile-2021.jpeg'
    }
  }
}
</script>

<style scoped>
.profile-frame{
  display: inline-block;
  width: 200px;
  height: 200px;
  overflow: hidden !important;
  background-position: center;
  background-size: 150%;
  background-repeat: no-repeat;
  border-radius: 100px;
  border:#fafafa6e 8px solid;
}
</style>