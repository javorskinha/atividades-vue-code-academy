<template>
    <p>counter {{ valor }} <br><button @click="incrementa">soma + 1</button></p>
</template>

<script setup>
import {ref} from 'vue'
    const mensagem = 'O contador chegou a dez'
    const valor = ref(0);
    function incrementa (){
        valor.value++
        if(valor.value === 10){
            emit('notificacao', mensagem)
        }
    }

    const emit = defineEmits(['notificacao'])

</script>

