<template>
  <div class="entry-level d-flex justify-content-between p-2">
    <div>
      <span class="text-success fs-5 fw-bold">15</span>
      <span class="mx-1 fs-5">Julio</span>
      <span class="mx-2 fw-light">2021, jueves</span>
    </div>
  </div>
  <div>
    <button class="btn btn-danger mx-2">
      Borrar
      <i class="fas fa-trash"></i>
    </button>

    <button class="btn btn-primary">
      Subir foto
      <i class="fas fa-upload"></i>
    </button>
  </div>
  <hr>
  <div class="d-flex flex-column px-3 h-75">
    <textarea
      placeholder="¿Qué ha pasado hoy?"
    ></textarea>
  </div>

  <FabIcon
    class="fab-icon"
    icon="fa-save"
    size="fa-2x"
    color="primary"
  />

  <img 
    src="https://picsum.photos/200/300"
    alt="entry-picture"
    class="img-thumbnail"
  />
</template>

<script>
import { defineAsyncComponent } from 'vue';
export default {
  components: {
    FabIcon: defineAsyncComponent(() => import('../components/FabIcon')),
  }
}
</script>

<style scoped>
 textarea {
   border: none;
   outline: none;
   resize: none;
   font-size: 1.2rem;
   font-family: 'Roboto', sans-serif;
   height: 100%;
   width: 100%;
   &:focus {
      outline: none;
   }
  }
   img {
     width: 200px;
     position: fixed;
     bottom: 150px;
     right: 20px;
     box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
   }
</style>