<template>
  <h2>Aula - 20</h2>
  <p>Aula de {{ aula }}</p>
  <Info/>
</template>

<script>
import Info from './info.vue';
export default {
  name: 'Aula',
  data(){
    return {
      aula: "Propriedade Computada"
    }
  },
  components: {
    Info
  }
}
</script>