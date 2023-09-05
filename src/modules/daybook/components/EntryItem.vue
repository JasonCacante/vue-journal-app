<template>
  <div 
    class="entry-container mb-3 pointer p-2"
    @click="$router.push({ name: 'entry', params: { id: 10 } })"
  >
    <div class="entry-title d-flex">
      <span class="text-success fs-5 fw-bold">15</span>
      <span class="mx-1 fs-5">Julio</span>
      <span class="mx-2 fw-light">2021, jueves</span>
    </div>
    <div class="entry-description">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex enim nulla delectus similique sit debitis nobis. Animi velit debitis similique reprehenderit consectetur, tempore aliquam numquam in accusamus atque! Perspiciatis, nisi?
    </div>
  </div>
</template>

<script>
  export default {

}
</script>

<style lang="scss">
.entry-container{
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0px 0px 10px rgba(0,0,0,0.2);
  cursor: pointer;
  transition: all 0.3s ease;

  &:hover {
    box-shadow: 0px 0px 14px rgba(0,0,0,0.4);
    background-color: lighten($color: grey, $amount: 45);
    transition: all 0.3s ease-in;
  }
  
  .entry-description {
    color: #2c3e50;
    font-size: 14px;
    padding: 10px;
    text-align: justify;
  }
}

</style>
