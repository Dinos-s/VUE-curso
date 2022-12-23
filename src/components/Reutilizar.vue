<template>
    <div>
        <button @click="ativar">Ativar</button>
        <span v-show="gtp">PRONTO</span>
    </div>
</template>

<style scoped>
    div{
        margin: 15px;
    }
</style>

<script>
    export default{
        name: 'Reutilizar',
        data(){
            return{
                gtp: false
            }
        },
        methods: {
            ativar(){
                this.gtp = !this.gtp
            }
        }
    }
</script>