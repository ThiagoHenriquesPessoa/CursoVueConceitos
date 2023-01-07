<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contatos</a></li>
    </ul>
</template>

<script>

export default {
    name: 'HeaderComponente'
}
</script>

<style scoped>
ul{
    list-style: none;
    display: flex;
    background-color: black;
}

li{
    margin-right: 10px;
}

a{
    color: #ddd;
    text-decoration: none;
    transition: .5s;
}

a:hover{
    color: blue;
}
</style>
