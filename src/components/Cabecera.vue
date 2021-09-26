<template>
<div class="row">
  <header class="bg-dark py-5">
    <div class="container px-5">
      <div class="row gx-5 justify-content-center">
        <div class="col-lg-6">
          <div class="text-center my-2">
            <h1 class="display-5 fw-bolder text-white mb-2">Fortalezcamos a diario los enlaces</h1>
            <p class="lead text-white-50 mb-4">Para lograr metas y propósitos en la vida es necesario enlazar emociones, esfuerzos y mil cosas más.</p>
            <div class="d-grid gap-3 d-sm-flex justify-content-sm-center">
              <a class="btn btn-primary btn-lg px-4 me-sm-3" v-on:click="sumaDiez">{{primero}}</a>
              <a class="btn btn-outline-light btn-lg px-4" v-on:click="sumaUno">{{segundo}}</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</div>
</template>

<script>
export default {
  name: "Cabecera",
  data(){
    return{
      primero:1,
      segundo:10
    }
  },
  methods:{
    sumaDiez:function (){
      this.segundo=this.segundo+10;
    },
    sumaUno:function (){
      this.primero=this.primero+1;
    }
  }
}
</script>

<style scoped>

</style>