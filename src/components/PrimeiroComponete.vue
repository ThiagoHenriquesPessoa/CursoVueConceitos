<template>
<h1>Olá Mundo!</h1>
<p>Meu nome é {{ name }} e trabalho como {{ profissao }}</p>
<MultiplosEventos/>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';

export default {
    name: 'PrimeiroComponete',
    components: {
        MultiplosEventos
    },
    data(){
        return{
            name: "Thiago",
            profissao: "Dev .Net, Vue e Angular junior"
        }
    }
    
}
</script>
