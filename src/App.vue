<template>
  <div id="app">
    <BarraNavegacion/>
    <Cabecera/>
    <div class="container-fluid">
    <div class="row">
        <Formulario/>
        <Carrusel/>
    </div>
      <PiePagina/>
    </div>
  </div>
</template>

<script>
import BarraNavegacion from "./components/BarraNavegacion.vue";
import Cabecera from "@/components/Cabecera";
import Formulario from "@/components/Formulario";
import Carrusel from "@/components/Carrusel";
import PiePagina from "@/components/PiePagina";
export default {
  name: 'App',
  components: {
    BarraNavegacion,
    Cabecera,
    Formulario,
    Carrusel,
    PiePagina
  }
}
</script>

<style>
</style>
