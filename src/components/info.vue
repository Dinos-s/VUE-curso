<template>
    <!-- <h2>Aula - 10</h2> -->
    <p>Usando o <strong>v-bind</strong> para alterar links de sites e src, isso é usado para deixar os componentes de forma dinamica, tambem pode ser usado com <strong>:+atributo htlm</strong></p>
    <p>Acesse o meu github e veja o meu trabalho <a v-bind:href="github" target="_blank">Dinos-s</a></p>
    <Picture/>
</template>

<script>
    import Picture from "./Picture.vue";
    export default {
        name: 'Info',
        components:{
            Picture,
        },
        data(){
            return {
                github:'https://github.com/Dinos-s',
            }
        }
    }
</script>