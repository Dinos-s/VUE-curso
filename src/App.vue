<template>
  <h1>Iniciando no Vue.JS</h1>
  <firstComponent/>
  <LifeCycle/>
  <Pessoa/>
</template>

<script>
import firstComponent from "./components/firstComponent.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";
  export default {
    name: 'App',
    components:{
      firstComponent,
      LifeCycle,
      Pessoa,
    },
  }
</script>