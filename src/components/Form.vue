<template>
    <div>
        <h2>Meu Formulario:</h2>
        <form action="" @submit="enviarform">
            <div>
                nome:<input type="text" v-model="name"><br>
                enviar:<input type="submit" name="">            
            </div>
        </form>
    </div>
</template>

<script>
export default {
    name:'Form',
    components: {

    },
    data(){
        return {
            name:''
        }
    },
    methods: {
        enviarform(e){

            e.pre

            const name = this.name;

            console.log('o nome é' + name)
        }
    }
}
</script>