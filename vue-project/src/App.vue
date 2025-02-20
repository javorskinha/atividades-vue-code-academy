<script setup>
import VmodelData from './components/VmodelData.vue'
import PropsPersonalizada from './components/PropsPersonalizada.vue'
import CompContador from './components/CompContador.vue'
</script>

<template>
  <h1>Olá</h1>
  <VmodelData/>
  <PropsPersonalizada nome="Rafael"/>
  <hr>
  <CompContador v-if="valor==10"/>
</template>

<style>

</style>
