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
    <div>
        <button @click="showEmail">{{botao_email}}</button>
    </div>
    <p >mande uma mensagem para: <a v-show="email">{{ email }}</a></p>
    <p class="link">Para acessar meu portfólio <a v-bind:href="meu_link">basta clicar aqui</a></p>
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
        mostrar_email: false,
        email: '',
        meu_link: 'https://google.com',
        botao_email: 'Mostrar e-mail'
    }
   },
   methods:{
    showEmail(){
        if(this.botao_email === 'Mostrar e-mail'){
            this.email = 'thiago@gmail.com'
            this.botao_email = 'Ocultar e-mail'
        }else{
            this.email = ''
            this.botao_email = 'Mostrar e-mail'
        }
    }
}
})
</script>
