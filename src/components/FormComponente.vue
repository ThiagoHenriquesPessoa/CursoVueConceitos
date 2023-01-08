<template>
    <form action="" @submit="enviarFormulario($event)">
        <input type="text" v-model="name">
        <input type="text" v-model="email">
       <div><SubmitForm/></div>
        
    </form>
</template>

<script>
import SubmitForm from './form/SubmitForm.vue';
export default{
    name: 'FormComponente',
    components:{
        SubmitForm
    },
    data(){
        return{
            name: '',
            email: ''
        }
    },
    methods: {
        enviarFormulario(e){
            e.preventDefault();

            const name = this.name;
            const email = this.email;

            console.log("Formulario enviado");    
            console.log("Nome: " + name); 
            console.log("E-mail: " + email);       
        }
    }
}
</script>