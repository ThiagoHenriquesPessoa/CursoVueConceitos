<template>
  <div class="container">
    <div class="box">
      <div class="box-cell box1">
        <HeaderComponente />
        <PrimeiroComponete />
        <LifeCycle />            
        <PessoaComponente />
      </div>
    </div>
  </div>
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
  text-align: center;
}
a{
  color: red;
}
.link{
  background-color: black;
  color: aqua;
}
.container .box {
  display: flex;
  flex-direction: row;
  text-align: center;
}
.container .box .box-cell.box1 {
  background: green;
  color: white;
  text-align: center;
}

.container .box .box-cell.box2 {
  background: lightgreen;
  text-align: center;
}
</style>
