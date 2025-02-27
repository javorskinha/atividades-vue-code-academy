<template>
    <div>
        <button @click="$emit('mudaFoto')">Mostrar dashboard </button>
    </div>
</template>

<script setup>
    const emit = defineEmits(['mudaFoto'])
</script>

<style>
    button {
        margin: 15px;
    }
</style>






