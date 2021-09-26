<template>
  <li class="nav-item">
    <a class="nav-link active" aria-current="page" :href="enlace.ruta">{{enlace.nombre}}</a>
  </li>
</template>

<script>
export default {
  name: "OpcionCabecera",
  props:{
    enlace:Object
  }
}
</script>

<style scoped>

</style>