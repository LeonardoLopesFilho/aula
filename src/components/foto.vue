<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>

export default{
    name:'foto',
    data() {
        return {
            avatar:"/img/Tonin4.png",
            descricao:"Tonin"
        }
    }
}
</script>
