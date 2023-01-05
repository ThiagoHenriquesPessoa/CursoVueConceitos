<template>
    <img :src="avatar" :alt="descricao" height="250" width="250">
</template>

<script>
export default {
    name: 'PictureComponente',
    data() {
        return {
            avatar: "/img/1Perfil.jpg",
            descricao: "Thiago Henriques Pessoa"
        }
    }
}
</script>
