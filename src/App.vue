<template>
  <div>
    <Header />
    <primeiro/>
    <LifeCycle />
    <Pessoa />
  </div>  
</template>


<script>
  import Header from './components/header.vue'
  import Primeiro from './components/Primeiro.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'

  export default {
    name: 'App',
    components: {
      Header,
      Primeiro,
      LifeCycle,
      Pessoa
    }
  }

</script>

<style>
  body{
    background-color:#333;
    color: #fff;
  }
</style>