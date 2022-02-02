<template>
  <div>
    <Header />
    <primeiro/>
    <LifeCycle />
    <Pessoa />
    <Form />
  </div>  
</template>


<script>
  import Header from './components/header.vue'
  import Primeiro from './components/Primeiro.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'
  import Form from './components/Form.vue'

  export default {
    name: 'App',
    components: {
      Header,
      Primeiro,
      LifeCycle,
      Pessoa,
      Form
    }
  }

</script>

<style>
  body{
    background-color:#333;
    color: #fff;
  }
</style>