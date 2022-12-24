<template>
    <!-- <h2>Aula - 18</h2> -->
    <p>Usando o <strong>$emit</strong> podemos emtir um evento no componente pai. Esse evento pode ser ivocado por um método no componente pai. Nã se esqueça de informar o que o componete deve fazer.</p>
    <p>Acesse o meu github e veja o meu trabalho <a v-bind:href="github" target="_blank">Dinos-s</a></p>
    <div>
        <button @click="showEmail">{{ btnText }}</button>
    </div>
    <p v-show="showemail">Meu contato: {{ email }}</p>
    <p>{{ email }}</p>
    <Picture/>
</template>

<script>
    import Picture from "./Picture.vue";
    export default {
        name: 'Info',
        components:{
            Picture,
        },
        props:{
            email: String
        },
        data(){
            return {
                github:'https://github.com/Dinos-s',
                showemail: false,
                btnText: 'Mostrar e-mail',
            }
        },
        methods: {
            showEmail(){
                this.showemail = !this.showemail
                if (!this.showemail) {
                    this.btnText = 'Mostrar e-mail'
                } else {
                    this.btnText = 'Olcutar e-mail'
                }
            }
        }
    }
</script>

<!-- style global -->
<style>
    body{
        background-color:  cadetblue;
        color: whitesmoke;
    }
</style>