<template>
  <div class="mb-3 pointer p-2" @click="$router.push({name:'entry', params:{id:10}})">
    <!-- Titulo -->
    <div class="entry-title d-flex">
        <span class="text-success fs-5 fw-bold">20</span>
        <span class="mx-1 fs-5">Mayo</span>
        <span class="mx-2 fw-light">2024, Martes</span>
    </div>

    <div class="entry-description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque reprehenderit aliquid ut natus maxime modi laboriosam, velit laudantium quasi eos impedit expedita? Nisi quis doloribus nesciunt doloremque, facilis libero dignissimos?
    </div>
  </div>
</template>

<script> 
export default {

}
</script>

<style lang="scss" scoped>
.entry-container{
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover{
        background-color: lighten($color: grey, $amount: 45);
        transition: 0.2s all ease-in;
    }

    .entry-descripcion{
    font-size: 12px;
}
}


</style>