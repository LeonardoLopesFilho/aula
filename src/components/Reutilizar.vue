<template>
    <div>
        <button @click="ativar">Clique Aqui!</button>
        <span v-show="ativou">ativado!</span>
    </div>
</template>

<script>
export default {
    name:'Reutilizar',
    data() {
        return {
            ativou:false
        }
    },
    methods: {
        ativar(){
            this.ativou = !this.ativou
        }
    }
}
</script>