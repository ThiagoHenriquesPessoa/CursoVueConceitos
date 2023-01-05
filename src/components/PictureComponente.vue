<template>
    <img :src="avatar" :alt="descricao" height="200" width="200">
</template>

<script>
export default {
    name: 'PictureComponente',
    data() {
        return {
            avatar: "/img/1Perfil.jpg",
            descricao: "Thiago Henriques"
        }
    }
}
</script>
