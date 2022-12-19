<template>
  <h1>Iniciando no Vue.JS</h1>
  <firstComponent/>
  <LifeCycle/>
</template>

<script>
import firstComponent from "./components/firstComponent.vue";
import LifeCycle from "./components/LifeCycle.vue";
  export default {
    name: 'App',
    components:{
      firstComponent,
      LifeCycle,
    },
  }
</script>