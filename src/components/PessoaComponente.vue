<template>
    <h2>Essa é a descrição de {{ nome }}</h2>
    <InfoComponente :compEmail="email"/>
    <FormComponente/>
</template>

<script>
import InfoComponente from './InfoComponente.vue'
import FormComponente from './FormComponente.vue';
export default{
    name: 'PessoaComponente',
    components:{
        InfoComponente,
        FormComponente
    },
    data(){
        return{
            nome: 'Thiago Henriques',
            email: 'henriques@gmail.com'
        }
    }
}
</script>