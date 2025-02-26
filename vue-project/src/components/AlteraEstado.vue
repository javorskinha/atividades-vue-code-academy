<template>
    <div>
        <ComponenteBotao v-if="exibeImagem" @click="mostrar(false)">{{texto}}</ComponenteBotao>
        <ComponenteBotao v-else @click="mostrar(true)" :texto="Exibir"/>
        <div v-if="exibeImagem">
            <img src="../../public/imgs/pirulito-azul.jpg" alt="" width="100px" height="75px">
            <img src="../../public/imgs/pirulito-rosa.jpg" alt=""
            width="100px" height="75px">
            <img src="../../public/imgs/pirulito-melancia.jpg" alt=""
            width="100px" height="75px">
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'
import ComponenteBotao from './ComponenteBotao.vue'
    const exibeImagem = ref(false)

    function mostrar (e){
        exibeImagem.value = e
    }
</script>