<template>
    <!-- Barra de navegacion -->
 <Navbar/>

 <div class="d-flex">
    <div class="col-4">
        <!-- seccion izquierda -->
       <EntryList/>
    </div>
    <div class="col">
        <!-- Contenido -->
        <router-view></router-view>
    </div>
 </div>
</template>

<script>
import {defineAsyncComponent} from 'vue'

export default {
    components:{
        Navbar: defineAsyncComponent(() => import('../components/Navbar.vue')),
        EntryList: defineAsyncComponent(() => import('../components/EntryList.vue')),
    }
}
</script>