<template>
    <div>
        <button @click="$emit('MudarImgComponente')">Trocar imagem do perfil</button>
    </div>
</template>
<script>


export default {
    name: 'MudarImgComponente',
    emits: ['MudarImgComponente'],
    methods: {
        TrocarImgComponente(){
            console.log('ops!');
    } 
}
}
</script>
