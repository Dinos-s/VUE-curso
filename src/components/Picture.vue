<template>
    <img :src="avatar" :alt="desc">
</template>

<script>
    export default {
        name: 'Picture',
        data(){
            return{
                avatar: "/img/avatar.png",
                desc: "User"
            }
        }
    }
</script>