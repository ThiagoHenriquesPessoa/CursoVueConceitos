<template>
  <PrimeiroComponete/>
  <LifeCycle/>
  <PessoaComponente/>
</template>

<script>
import PrimeiroComponete  from './components/PrimeiroComponete.vue'
import LifeCycle from './components/LifeCycle.vue'
import PessoaComponente from './components/PessoaComponente.vue';

export default {
    name: 'App',
    components:{
      PrimeiroComponete,
      LifeCycle,
      PessoaComponente
    }
}
</script>
