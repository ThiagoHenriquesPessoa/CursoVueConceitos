<template>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utiliso as seguintes tecnologias</p>
    <ul>
        <li>JavaScript</li>
        <li>TypeScript</li>
        <li>CSharp</li>
        <li>SqlServer</li>
    </ul>
    <p v-show="mostrar_email">mande uma mensagem para: {{ email }}</p>
    <p>Para acessar meu portfólio <a v-bind:href="meu_link">basta clicar aqui</a></p>
    <PictureComponente/>
</template>

<script>
import PictureComponente from './PictureComponente.vue'
export default ({
   name: 'InfoComponente',
   components: {
    PictureComponente
   },
   data(){
    return{
        esta_trabalhando: false,
        mostrar_email: true,
        email: 'thiago@gmail.com',
        meu_link: 'https://google.com'
    }
   }
})
</script>
