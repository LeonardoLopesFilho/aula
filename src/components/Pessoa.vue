<template>
    <div>
        <h2>Esta é a descrição da pessoa {{nome}}</h2>   
        <info :email="email" :trabalho = true />
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
            email:'leozaosacana@gmail.com'
        }
    }
}


</script>