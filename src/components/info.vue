<template>
    <!-- <h2>Aula - 14</h2> -->
    <p>São usados para complementar ações dos usários com a ativação dos métodos como vimos no <strong>@click()</strong> podendo receber parametros, para executar o determinado evento.</p>
    <p>Acesse o meu github e veja o meu trabalho <a v-bind:href="github" target="_blank">Dinos-s</a></p>
    <div>
       <button @click="showEmail">{{ btnText }}</button>
    </div>
    <p>Possuo conhecimeto em:</p>
    <p>Beckend:</p>
    <ul>
        <li v-for="(tecnology, index) in Tec_backend" :key="index">
            {{ tecnology }}
        </li>
    </ul>
    <p>Frontend:</p>
    <ul>
        <li v-for="tecnology in Tec_frotend" :key='tecnology.id'>
            {{ tecnology.lenguage }}
        </li>
    </ul>
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
                Tec_backend: ['JavaScript', "Python", `MySQL`],
                Tec_frotend: [
                    {id: 1, lenguage: 'HTML'},
                    {id: 2, lenguage: 'CSS'},
                    {id: 3, lenguage: 'JS'},
                ],
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