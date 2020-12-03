<template>
  <div class="card" style="width: 18rem">
    <img class="card-img-top" src="../assets/logo.png" alt="Card image cap" />
    <div class="card-body">
      <h5 class="card-title">{{integrante.nombre}}</h5>
      <p class="card-text">
        {{integrante.descripcion}}
      </p>
    </div>
  </div>
</template>

<script>
import integrante from '../integrantes.json'
export default {
  name: "TeamCard",
  props: ["member"],
  data(){
      return {
          integrante: integrante
      }
  }
};
</script>

<style scoped>
</style>
