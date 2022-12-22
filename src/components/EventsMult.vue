<template>
    <div>
        <button @click="Evet1(txt1, $event), Evet2($event)">Ativar Eventos Multiplos</button>
        <p>{{ MultsEvent }}</p>
    </div>
</template>

<style scoped>
    div{
        margin: 15px;
    }
</style>

<script>
    export default{
        name: 'EventsMult',
        data(){
            return{
                MultsEvent: '',
                txt1: 'Evento 1 ativado'
            }
        },
        methods: {
            Evet1(txt1, e){
                this.MultsEvent = txt1
            },
            Evet2(e){
                setTimeout(() => {
                    this.MultsEvent = 'Evento 2: ativado'
                }, 500);
            }
        }
    }
</script>