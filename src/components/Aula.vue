<template>
    <h2>Aula - 11</h2>
    <h2>Aula de {{ aula }}</h2>
    <Info/>
</template>

<script>
    import Info from "./info.vue";
    export default{
        name: 'aula',
        components:{
            Info,
        },
        data(){
            return {
                aula: 'Métodos'
            }
        }
    }
</script>