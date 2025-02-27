<script setup>
import VmodelData from './components/VmodelData.vue'
import PropsPersonalizada from './components/PropsPersonalizada.vue'
import CompContador from './components/CompContador.vue'
import MostraFotos from './components/MostraFotos.vue'
import MudaFoto from './components/MudaFoto.vue'

function recebeEvento(mensagem){
  window.alert(mensagem)
}
</script>

<template>
  <h1>Olá</h1>
  <VmodelData/>
  <PropsPersonalizada nome="Rafael"/>
  <hr>
  <CompContador @notificacao="recebeEvento"/>
  <hr>
  <MostraFotos/>
  <hr>
  <MudaFoto />
</template>

<style>

</style>
