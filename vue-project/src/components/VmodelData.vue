<template>
    <input type="text" placeholder="Digite seu nome" v-model="nome">
    <h1>Seja bem vindo {{ nome }}!</h1>
    <p>{{ nome }} que bom ver você por aqui.</p>
</template>

<script setup>
import {ref} from 'vue'

    const nome = ref('')

</script>


