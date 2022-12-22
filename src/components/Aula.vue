<template>
    <h2>Aula - 15</h2>
    <h2>Aula de {{ aula }}</h2>
    <Info/>
    <EventsMult/>
</template>

<style>
    a{
        color: red;
    }
</style>

<script>
    import Info from "./Info.vue";
    import EventsMult from './EventsMult.vue';
    export default{
        name: 'aula',
        components:{
            Info,
            EventsMult,
        },
        data(){
            return {
                aula: 'Eventos Multiplos'
            }
        }
    }
</script>