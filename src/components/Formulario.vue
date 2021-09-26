<template>
  <div class="col-md-6 p-2">
    <div class="card">
      <div class="card-header text-center">
        Formulario de envío de datos
      </div>
      <div class="card-body">
        <div class="mb-3">
        <label for="nombre" class="form-label">Nombre:</label>
        <input type="text" class="form-control" id="nombre" v-model="nombre" placeholder="Escriba su nombre aquí">
        </div>
        <div class="mb-3">
        <label for="direccion" class="form-label">Dirección:</label>
        <input type="text" class="form-control" id="direccion" placeholder="Dirección">
        </div>
        <div class="mb-3">
          <label for="comentarios" class="form-label">Comentarios:</label>
          <textarea class="form-control" id="comentarios" rows="3" placeholder="Cuéntanos algo..."></textarea>
        </div>
        <div class="d-grid gap-2">
          <button class="btn btn-primary" type="button" v-on:click="enviarInfo">Enviar</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios';
export default {
  name: "Formulario",
  data(){
    return{
      nombre:'',
      direccion:'',
      comentarios:''
    }
  },
  methods:{
    enviarInfo(){
      // let url='localhos/rcrr/Rest.php'
      // console.log(axios);
      // const usuario = {
      //   nombre: 'Roberto',
      //   direccion: 'Bajos del Ejido'
      // };
      axios.get(`http://localhost/rcrr/Rest.php`)
          .then(response => {
            console.log(response)
            // Obtenemos los datos
          })
          .catch(e => {
            // Capturamos los errores
            console.log(e)
          })
    }
  }
}
</script>

<style scoped>

</style>