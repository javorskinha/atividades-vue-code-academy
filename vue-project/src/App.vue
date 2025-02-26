<script setup>
import VmodelData from './components/VmodelData.vue'
import PropsPersonalizada from './components/PropsPersonalizada.vue'
import CompContador from './components/CompContador.vue'
import AlteraEstado from './components/AlteraEstado.vue'

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
  <AlteraEstado/>
</template>

<style>

</style>
