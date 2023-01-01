<template>
<h1>Olá Mundo!</h1>
<p>Meu nome é {{ name }} e trabalho como {{ profissao }}</p>
</template>

<script>

export default {
    name: 'PrimeiroComponete',
    data(){
        return{
            name: "Thiago",
            profissao: "Dev C# junior"
        }
    }
    
}
</script>
