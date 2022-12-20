<template>
    <h2>Aula - 07</h2>
    <h1>Animal: {{ animal }}</h1>
    ---------------------------------------

</template>

<script>
    export default {
        animal: 'Animal',
        data(){
            return{
                animal: 'desconhecido'
            }
        },
        
        created(){
            setTimeout(() => {
                this.animal = "Morcego"
            }, 1000);
        },

        mounted(){
            setTimeout(() => {
                this.animal = "T-Rex"
            }, 2000);
        }
    }
</script>