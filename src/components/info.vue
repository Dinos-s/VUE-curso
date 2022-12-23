<template>
    <!-- <h2>Aula - 17</h2> -->
    <p>Podendo receber dados, vindas pelo data() ou de modo mais direto, e assim como nos metódos, é nescessário criar um seção props.</p>
    <p>tbm podemos utilizar os props como arrays, e passar podemos passar mais de uma proprie dade por vez.</p>
    <p>Acesse o meu github e veja o meu trabalho <a v-bind:href="github" target="_blank">Dinos-s</a></p>
    <div>
        <button @click="showEmail">{{ btnText }}</button>
    </div>
    <p v-show="showemail">Meu contato: {{ email }}</p>
    <p>{{ email }}</p>
</template>

<script>
    export default {
        name: 'Info',
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