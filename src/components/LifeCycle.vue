<template>
    <h1>Animal: {{ animal }}</h1>
</template>

<script>
    export default {
        animal: 'Rino',
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