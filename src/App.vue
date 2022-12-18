<template>
  <h1>Iniciando no Vue.JS</h1>
  <firstComponent/>
</template>

<script>
import firstComponent from "./components/firstComponent.vue";
  export default {
    name: 'App',
    components:{
      firstComponent
    }
  }
</script>