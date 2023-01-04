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
</template>

<script>
export default ({
   name: 'InfoComponente',
   data(){
    return{
        esta_trabalhando: false,
        mostrar_email: false,
        email: 'thiago@gmail.com'
    }
   }
})
</script>
