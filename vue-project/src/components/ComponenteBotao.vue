<template>
    <button>{{ texto }}</button>
</template>

<script setup>
import { defineProps } from 'vue';
    const props = defineProps({texto: String})
</script>