<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li>
        <li v-if="logado"><a href="#">Meu Perfil</a></li>
    </ul>
</template>

<style scoped>
    ul{
        list-style: none;
        display: flex;
        background-color: darkgrey;
    }
    li{
        margin-right: 10px;
    }
    a{
        color: #DDD;
        text-decoration: none;
        transition: .5s;
    }
    a:hover{
        color: rgb(88, 64, 224);
    }
</style>

<script>
    export default{
        name: 'Header',
        props: ['logado'] //ñ é nesssésario a declaração da sua tipagem
    }
</script>