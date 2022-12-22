<template>
    <h2>Aula - 14</h2>
    <h2>Aula de {{ aula }}</h2>
    <Info/>
    <Form/>
</template>

<style>
    a{
        color: red;
    }
</style>

<script>
    import Info from "./Info.vue";
    import Form from './Form.vue';
    export default{
        name: 'aula',
        components:{
            Info,
            Form
        },
        data(){
            return {
                aula: 'Eventos'
            }
        }
    }
</script>