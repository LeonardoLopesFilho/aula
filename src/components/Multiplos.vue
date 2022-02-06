<template>
    <div>
        <button @click="primeiro($event),segundo()">Ativar Multiplos Eventos</button>
        <p>{{multiplos}}</p>
    </div>
</template>

<script>
export default {
    name:'Multiplos',
    data() {
        return {
            multiplos:"",
            
        }
    },
    methods:{
        primeiro(){
            this.multiplos = "Primeiro Evento"
        },
        segundo(){
            setTimeout(() =>this.multiplos = "Segundo Evento!",500)
        }
    }
}
</script>