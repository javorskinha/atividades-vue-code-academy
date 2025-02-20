<template>
    <p>counter {{ valor }} <br><button @click="incrementa">soma + 1</button></p>
    <p>{{mensagem}}</p>
</template>

<script setup>
import {ref} from 'vue'
    const mensagem = ''
    const valor = ref(0);
    function incrementa (){
        valor.value++
    }
</script>

