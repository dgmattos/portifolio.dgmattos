<template>
  <div>
    <div class="profile-frame" :style="{backgroundImage:'url(' + src + ')'}">
    </div>
    <h1 class="text-white mt-3">DEIVID GUSTAVO MATTOS</h1>
  </div>
</template>

<script>
export default {
  name: "profilePic",
  props:{
    src:{
      type:String,
      default:''
    },
    alt:{
      type:String,
      default:'img alt'
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
