<script setup>
import { ref } from 'vue';
import VmodelData from './components/VmodelData.vue'
import PropsPersonalizada from './components/PropsPersonalizada.vue'
import CompContador from './components/CompContador.vue'
import MostraFotos from './components/MostraFotos.vue'
import MudaFoto from './components/MudaFoto.vue'
import PercorreArray from './components/PercorreArray.vue'

function recebeEvento(mensagem){
  window.alert(mensagem)
}

    const corInicial = ref('')

</script>

<template>
  <div :style="{backgroundColor: corInicial}">
    <h1>Olá</h1>
    <VmodelData/>
    <PropsPersonalizada nome="Rafael"/>
    <hr>
    <CompContador @notificacao="recebeEvento"/>
    <hr>
    <MostraFotos/>
    <hr>
    <MudaFoto />
    <PercorreArray />
    <hr>
    <input type="color" v-model="corInicial">
  </div>
</template>

<style>

</style>