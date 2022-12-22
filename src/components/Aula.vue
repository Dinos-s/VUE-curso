<template>
    <h2>Aula - 13</h2>
    <h2>Aula de {{ aula }}</h2>
    <Info/>
</template>

<style>
    a{
        color: red;
    }
</style>

<script>
    import Info from "./Info.vue";
    export default{
        name: 'aula',
        components:{
            Info,
        },
        data(){
            return {
                aula: 'Listas(v-for)'
            }
        }
    }
</script>