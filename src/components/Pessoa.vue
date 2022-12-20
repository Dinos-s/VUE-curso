<template>
    <h2>Aula - 09</h2>
    <h2>Eu sou {{ nome }}</h2>
    <Info/>
</template>

<script>
    import Info from "./info.vue";
    export default{
        name: 'Pessoa',
        components:{
            Info,
        },
        data(){
            return {
                nome: 'GMR'
            }
        }
    }
</script>