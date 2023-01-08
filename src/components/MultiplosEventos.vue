<template>
    <div>
        <button @click="primeiro(txt1), segundo(txt2), terceiro()">Ativando multiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>
<script>

export default {
    name: 'MultiplosEventos',
    data() {
        return{
        multiplos_eventos: "",
        txt1: "Primeiro evento ativado!",
        txt2: "Segundo evento ativado!"
        }
    },
    methods:{
        primeiro(txt){
            this.multiplos_eventos = txt
        },
        segundo(txt){
            setTimeout(() => this.multiplos_eventos = txt, 1000)
        },
        terceiro(){
            setTimeout(() => this.multiplos_eventos = "", 2000)
        }
    }
}
</script>
<style scoped>
div{
    margin: 100px;
}
</style>
