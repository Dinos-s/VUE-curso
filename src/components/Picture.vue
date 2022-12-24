<template>
    <img :src="avatar" :alt="desc">
    <MudarImagem @mudar-imagem="trocarImagem"/>
</template>

<script>
    import MudarImagem from "./MudarImg.vue";
    export default{
        name: 'Picture',
        components:{
            MudarImagem
        },
        data(){
            return{
                avatar: "/img/avatar.png",
                desc: 'User'
            }
        },
        methods:{
            trocarImagem(){
                this.avatar = '/img/avatar2.png';
            }
        }
    }
</script>