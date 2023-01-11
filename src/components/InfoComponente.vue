<template>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades</p>

    <p>Utiliso as seguintes tecnologias para back-end:</p>
    <ul>
        <li v-for="(technology, index) in backend_technologies" v-bind:key="index">{{technology}} - Back-End</li>
    </ul>
    <p>Utiliso as seguintes tecnologias para front-end:</p>
    <ul>
        <li v-for="technology in frontend_technologies" v-bind:key="technology.id">{{technology.language}} - Front-End</li>
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
        botao_email: 'Mostrar e-mail',
        backend_technologies: ['JavaScript', 'TypeScript', 'CSharp', 'SqlServer'],
        frontend_technologies:[
            {id:1, language:'HTML'},
            {id:2, language:'CSS'},
            {id:3, language:'JavaScript'},
            {id:4, language:'TypeScript'},
            {id:5, language:'Vue'},
            {id:6, language:'Angular'}
        ]
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
