<template>
    <img :src="avatar" :alt="descricao" height="250" width="250">
    <MudarImgComponente @mudar-imgComponente="TrocarImgComponente"/>
</template>

<script>
import MudarImgComponente from './MudarImgComponente.vue'

export default {
    name: 'PictureComponente',
    components:{
        MudarImgComponente
    },
    data() {
        return {
            avatar: "",
            descricao: "Thiago Henriques Pessoa"
        }
    },
    methods: {
        TrocarImgComponente(){
            if(this.avatar === "/img/1Perfil.jpg"){
                this.avatar = "/img/2Perfil.jpg"
            }else{
                this.avatar = "/img/1Perfil.jpg"
            }
            
    } 
}
}
</script>
