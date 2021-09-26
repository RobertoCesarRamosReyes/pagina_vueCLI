<template>
  <div class="row">
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container px-5">
      <a class="navbar-brand" href="#!">Linking</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"><span class="navbar-toggler-icon"></span></button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
          <OpcionNav v-for="(enlace,index) in enlaces" :key="index" :enlace="enlace" />
        </ul>
      </div>
    </div>
  </nav>
  </div>
</template>

<script>
import OpcionNav from "./OpcionNav";
export default {
  name: "BarraNavegacion",
  components:{
    OpcionNav
  },
  data(){
    return{
      enlaces: [
        {nombre:'Inicio',ruta:'home.php'},
        {nombre:'Conocenos',ruta:'about.php'},
        {nombre:'Contáctanos',ruta:'contact.php'},
        {nombre:'Servicios',ruta:'services.php'},
      ]
    }
  }
}
</script>

<style scoped>

</style>