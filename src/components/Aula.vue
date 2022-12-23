<template>
    <Header :logado="true"/>
    <h2>Aula - 17</h2>
    <h2>Aula de {{ aula }}</h2>
    <Info :email="email"/>
</template>

<style>
    a{
        color: red;
    }
</style>

<script>
    import Info from "./Info.vue";
    import Header from "./Header.vue";
    export default{
        name: 'aula',
        components:{
            Info,
            Header,
        },
        data(){
            return {
                aula: 'Props',
                email: "LTP7@gmail.com"
            }
        }
    }
</script>