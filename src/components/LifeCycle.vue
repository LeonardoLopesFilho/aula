<template>
    <div class="container">
        <h1> Meu nome é: {{nome}}</h1>
    </div>
</template>

<script>

export default{
    name : 'LifeCycle' ,
    data(){
        return{
            nome: 'Ainda Não sei'
        }
    },
    created(){
        setTimeout(() =>{
            this.nome = 'Leozao'
        }, 1000);
       },
    mounted(){
        setTimeout(() =>{
            this.nome = 'sacana'
        }, 2000);
    }
}

</script>