<template>
    <h2>Aula - 16</h2>
    <h2>Aula de {{ aula }}</h2>
    <Info/>
    <p>Componente Aula:</p>
    <Reutilizar/>
</template>

<style>
    a{
        color: red;
    }
</style>

<script>
    import Info from "./Info.vue";
    import Reutilizar from './Reutilizar.vue';
    export default{
        name: 'aula',
        components:{
            Info,
            Reutilizar,
        },
        data(){
            return {
                aula: 'Reutilizar Componentes'
            }
        }
    }
</script>