<template>
    <!-- <h2>Aula - 15</h2> -->
    <p>Assim como na aula14, tbm temos os eventos multiplos, isso que dizer, que em um determinado momento ou em um botão, podemos invocar mais de um evento no template.</p>
    <p>Acesse o meu github e veja o meu trabalho <a v-bind:href="github" target="_blank">Dinos-s</a></p>
    <p v-show="showemail">Meu contato: {{ email }}</p>
</template>

<script>

    export default {
        name: 'Info',
        data(){
            return {
                github:'https://github.com/Dinos-s',
                email: 'info@.com',
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