<template>
  <div class="d-flex justify-content-center">
    <h1 class="align-self-center">No hay nada seleccionado</h1>
  </div>
  <FabIcon />
</template>

<script>
import { defineAsyncComponent } from 'vue';
export default {
  components: {
    FabIcon: defineAsyncComponent(() => import(/* webpackChunkName: "daybook-fab" */'../components/FabIcon.vue')),
  }
}
</script>

<style lang="scss" scoped>
div {
  height: 100%;
}
</style>