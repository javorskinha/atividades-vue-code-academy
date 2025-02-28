<template>
    <div>
        <h1>Lista de Mercado:</h1>
        <button @click="exibe()">exibir lista</button>
        <ul type="square" v-if="mostrar">
            <li v-for="item in lista" :key="item.id">{{ item.nome }}</li>
        </ul>
    </div>
</template>

<script setup>
import { ref } from 'vue'

    const lista = ref([
        {id: 1, nome: "pão"},
        {id: 2, nome: "leite"},
        {id: 3, nome: "ovos"},
        {id: 4, nome: "trigo"},
        {id: 5, nome: "arroz"},
        {id: 6, nome: "feijão"},
        {id: 7, nome: "alface"},
        {id: 8, nome: "brócolis"},
        {id: 9, nome: "batata"},
        {id: 10, nome: "carne"}
    ])

    const mostrar = ref(false)

    function exibe(){
        mostrar.value = !mostrar.value
    }

</script>





