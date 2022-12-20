<template>
    <h2>Aula - 08</h2>
    <h2>Eu sou {{ nome }}</h2>
    <Info/>
    <Form/>
    ---------------------------------------
</template>

<script>
    import Info from "./info.vue";
    import Form from "./Form.vue";
    export default{
        name: 'Pessoa',
        components:{
            Info,
            Form,
        },
        data(){
            return {
                nome: 'GMR'
            }
        }
    }
</script>