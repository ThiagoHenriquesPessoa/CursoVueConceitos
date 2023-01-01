<template>
  <PrimeiroComponete/>
  <LifeCycle/>
</template>

<script>
import PrimeiroComponete  from './components/PrimeiroComponete.vue'
import LifeCycle from './components/LifeCycle.vue'

export default {
    name: 'App',
    components:{
      PrimeiroComponete,
      LifeCycle
    }
}
</script>
