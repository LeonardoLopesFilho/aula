<template>
    <div class="">
        <h1>Olá Vue!</h1>
        <p>Meu Nome é {{ nome }} e trabalho com {{ profissao }}</p>
    </div>    
</template>

<script>
    export default {
        name:'Primeiro',
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
