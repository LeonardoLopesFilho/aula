<template>
    <div>
        <p v-if="trabalho">Estou Trabalhando no momento.</p>
        <p v-else>Estou em Busca de Novas Oportunidades</p>
        <p>Utilizo as seguintes tecnologias</p>
        <ul >
            <li v-for="(tech,index) in backend" v-bind:key="index">{{tech}}</li>
        </ul> 
         <p>Utilizo as seguintes tecnologias para frontend</p>
         <ul >
            <li v-for="tech in frontend" v-bind:key="tech.id">{{tech.linguagem}}</li>
        </ul> 
        <div>
            <button @click="showEmail">Mostrar Email</button>
        </div>

        <p v-show="motraremail">Mande uma mensagem para {{email}}</p>
        <p>Para Acessar o meu portifolio <a v-bind:href="meu_link">{{textobotao}}</a></p>
        <foto />
    </div>
</template>

<script>

import foto from './foto.vue';

export default {
    nome:'info',
    components:{
        foto
    },
    props:{
        email: String,
        trabalho:Boolean
    },
    data(){
        return {
            motraremail: false,
            meu_link:'https://google.com',
            textobotao : "Mostrar Email",
            backend:["PHP","PYTHON","Laravel","SQL"],
            frontend:[
                {id:1,linguagem:'HTML'},
                {id:2,linguagem:'JS'},
                {id:3,linguagem:'CSS'}
            ]
        }
    },
    methods: {
        showEmail(){
            this.motraremail = !this.motraremail
            if(!this.motraremail){
                this.textobotao = 'Mostrar Email'
            }else{
                this.textobotao = 'Esconder Email'
            }

        }
    }
}
</script>