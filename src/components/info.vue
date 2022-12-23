<template>
    <!-- <h2>Aula - 16</h2> -->
    <p>Assim com já foi dito, componetes podem ser reutilizados, em outras partes no código, sem a menor interferência, entre elas.</p>
    <p>Acesse o meu github e veja o meu trabalho <a v-bind:href="github" target="_blank">Dinos-s</a></p>
    <p v-show="showemail">Meu contato: {{ email }}</p>

    <p>Componente Info:</p>
    <Reutilizar/>
</template>

<script>
    import Reutilizar from "./Reutilizar.vue";
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
        components: {
            Reutilizar,
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