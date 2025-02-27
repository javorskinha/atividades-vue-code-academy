<template>
    <div>
        <MandaEvento @mudaFoto="trocaFoto"/>
        <img :src="foto" alt="">
    </div>
</template>

<script setup>
import { ref } from 'vue';
import MandaEvento from './MandaEvento.vue';

    const foto = ref("../../public/imgs/vue-icone.jpg")

    function trocaFoto(){
        foto.value = "../../public/imgs/vue-dashboard.jpg"
    }

</script>






