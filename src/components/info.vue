<template>
    <!-- <h2>Aula - 09</h2> -->
    <p v-if="nao_trabalhando">No momento estou a procura de novas oprtunidades de emprego</p>
    <p v-else>No momento estiu trabalhando com <strong>Vue.js</strong></p>
    <p>Possuo conhecimeto em:</p>
    <ul>
        <li>JavaScript</li>
        <li>HTML</li>
        <li>MySQL</li>
        <li>Vue.js</li>
    </ul>
    <p v-show="showEmail">email para contato: {{ email }}</p>
</template>

<script>
    export default {
        name: 'Info',
        data(){
            return {
                nao_trabalhando: false,
                email: 'info@.com',
                showEmail: true,
            }
        }
    }
</script>