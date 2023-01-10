<template>
    <div>
        <button @click="ativar">Clique aqui!</button>
        <span v-show="ativou">{{activ}}</span>
    </div>
</template>
<script>


export default {
    name: 'ReutilizacaoComponente',
    data(){
        return{
            ativou: false,
            activ: "Ativado!"
        }
    },
    methods:{
        ativar(){
        this.ativou = !this.ativou
        }
    }
}
</script>
