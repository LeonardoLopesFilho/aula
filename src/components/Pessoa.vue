<template>
    <div>
        <h2>Esta é a descrição da pessoa {{nome}}</h2>   
        <info />
    </div>
</template>

<script>

import info from './info.vue'

export default{
    name: 'Pessoa',
    components: {
        info
    },
    data(){
        return{
            nome: 'Leonardo',
        }
    }
}


</script>