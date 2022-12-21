<template>
    <!-- <h2>Aula - 12</h2> -->
    <p>No parte de estilização o <strong>CSS</strong> pode ser declarado de dois modos o global, que é apenas a tag css declarada no final do codigo vue.</p>
    <p>Já no scopo é nescessário declarar a tag css com o atributo scode, assim o css será isolado somente aquele componente.</p>
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

<!-- style global -->
<style>
    body{
        background-color:  cadetblue;
        color: whitesmoke;
    }
</style>