<template>
    <h2>Essa é a descrição de {{ nome }}</h2>
    <InfoComponente/>
</template>

<script>
import InfoComponente from './InfoComponente'
export default{
    name: 'PessoaComponente',
    components:{
        InfoComponente
    },
    data(){
        return{
            nome: 'Thiago'
        }
    }
}
</script>