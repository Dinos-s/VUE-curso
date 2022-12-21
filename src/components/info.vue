<template>
    <!-- <h2>Aula - 11</h2> -->
    <p>Basicamente funções que podem ser executadas em eventos ou uma lógica. Podendo ser chamados pelo <strong>@click</strong> em um butão, que executará o método, determinado, os metodos são tratados como objeto.</p>
    <p><strong>Use o 'this.', para manipular o seu metodo</strong></p>
    <p>Acesse o meu github e veja o meu trabalho <a v-bind:href="github" target="_blank">Dinos-s</a></p>
    <div>
        <button @click="showEmail">{{ btnText }}</button>
    </div>
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
                btnText: 'Mostrar e-mail'
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