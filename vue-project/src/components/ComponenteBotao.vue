<template>
    <button>{{ texto }}</button>
</template>

<script>
import { defineProps } from 'vue';
    defineProps({texto: String})
</script>