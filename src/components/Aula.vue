<template>
    <h2>Aula - 12</h2>
    <Header/>
    <h2>Aula de {{ aula }}</h2>
    <Info/>
</template>

<style>
    a{
        color: red;
    }
</style>

<script>
    import Info from "./info.vue";
    import Header from './Header.vue';
    export default{
        name: 'aula',
        components:{
            Info,
            Header
        },
        data(){
            return {
                aula: 'CSS'
            }
        }
    }
</script>