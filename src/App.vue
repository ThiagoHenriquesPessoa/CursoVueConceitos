<template>
  <HeaderComponente/>
  <PrimeiroComponete/>
  <LifeCycle/>
  <PessoaComponente/>
</template>

<script>
import HeaderComponente from './components/HeaderComponente.vue';
import PrimeiroComponete  from './components/PrimeiroComponete.vue'
import LifeCycle from './components/LifeCycle.vue'
import PessoaComponente from './components/PessoaComponente.vue';

export default {
    name: 'App',
    components:{
      HeaderComponente,
      PrimeiroComponete,
      LifeCycle,
      PessoaComponente
    }
}
</script>

<style>
body{
  background-color: #333;
  color: #fff;
}
a{
  color: red;
}

.link{
  background-color: black;
  color: aqua;
}
</style>
