<template>
    <div class="">
        <h1>Olá Vue!</h1>
        <p>Meu Nome é {{ nome }} e trabalho com {{ profissao }}</p>
        <Multiplos />
        <Reutilizar />
        <Reutilizar />
    </div>    
</template>

<script>
import Multiplos from './Multiplos.vue'
import Reutilizar from './Reutilizar.vue'
    export default {
        name:'Primeiro',
        components:{
            Multiplos,
            Reutilizar
        },
        data(){
            return {
                nome:"Leonardo",
                profissao: "Programador"
            }
        }
    }
</script>

<style>

</style>
