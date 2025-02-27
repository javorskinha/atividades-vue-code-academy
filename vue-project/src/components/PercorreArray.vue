<template>
    <div>
        <ul>
            <li>{{  }}</li>
        </ul>
    </div>
</template>

<script>
import { ref } from 'vue'
    const id = ref('')

    const nome = ref('')

    async function getLista (){
        const req = await fetch('http://localhost:3000/lista')

        const data = await req.json()

        id = data.id
        nome = data.nome
    }

</script>





