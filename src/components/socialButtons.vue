<template>
  <div class="btn-group" role="group" aria-label="Basic example">
    <a class="px-2 fs-4" target="_blank" v-for="item in redes" :key="item.label" :href="item.url" :title="item.label" data-bs-toggle="tooltip" data-bs-placement="bottom">
      <span class="text-fantasma" v-html="item.icon"></span>
    </a>
  </div>
</template>

<script>
export default {
  name: "socialButtons",
  created() {

  },
  mounted() {
    this.redes.push({icon:'<i class="fab fa-whatsapp"></i>',label:'+55 27 9 8153 9221',url:'https://api.whatsapp.com/send?phone=5527981539221&text=Ol%C3%A1%20Deivid,%20tudo%20bem?%20Vi%20seu%20portif%C3%B3lio%20e%20estou%20entrando%20em%20contato%20para%20%C2%A0'})
    this.redes.push({icon:'<i class="fas fa-envelope"></i>',label:'deivid@dgmattos.com.br',url:'mailto:deivid@dgmattos.com.br'})
    this.redes.push({icon:'<i class="fab fa-instagram"></i>',label:'@deividgmattos',url:'https://www.instagram.com/deividgmattos/'})
    this.redes.push({icon:'<i class="fab fa-facebook"></i>',label:'@deividgmattos',url:'https://www.facebook.com/deividgmattos'})
    this.redes.push({icon:'<i class="fab fa-linkedin"></i>',label:'deivid-mattos-77373516b',url:'https://www.linkedin.com/in/deivid-mattos-77373516b/'})
    this.redes.push({icon:'<i class="fab fa-github"></i>',label:'@dgmattos',url:'https://github.com/dgmattos/'})
    this.redes.push({icon:'<i class="fas fa-globe"></i>',label:'dgmattos.com.br',url:'https://dgmattos.com.br/'})
  },
  data:function(){
    return{
      redes:[]
    }
  }
}
</script>

<style scoped>

</style>