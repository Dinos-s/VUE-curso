<template>
    <!-- <h2>Aula - 20</h2> -->
    <div>
        <p>De modo resumido, as propriedades computadas são funções que dependem de outros componentes, para o valor final ser apresentado;</p>
        <p>Durante o uso das props computadas, os dados/valores finais só serão executadas caso um dos valores dependentes seja alterado. já que esses daos são amarzenados em cash.</p>

        First Name:
        <input type="text" v-model="user.Fname"><br>
        Last Name:
        <input type="text" v-model="user.Lname">
        <p>Nome completo: {{ fullName }}</p>
    </div>
</template>

<script>
export default {
    name: "Info",
    data() {
        return {
            user: {
                Fname: '',
                Lname: ''
            }
        }
    },
    computed: {
        fullName(){
            return `${this.user.Fname} ${this.user.Lname}`
            
        }
    }
}
</script>