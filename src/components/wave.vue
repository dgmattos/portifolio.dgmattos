<template>
  <div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path :fill="fill" fill-opacity="1" d="M0,224L60,240C120,256,240,288,360,293.3C480,299,600,277,720,245.3C840,213,960,171,1080,170.7C1200,171,1320,213,1380,234.7L1440,256L1440,0L1380,0C1320,0,1200,0,1080,0C960,0,840,0,720,0C600,0,480,0,360,0C240,0,120,0,60,0L0,0Z"></path></svg>
  </div>
</template>

<script>
export default {
  name: "wave",
  props:{
    fill:{
      default:'#2c3e50'
    }
  }
}
</script>

<style scoped>

</style>
