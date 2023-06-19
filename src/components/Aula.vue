<template>
  <h2>Aula - 22</h2>
  <p>Aula de {{ aula }}</p>
  <Info>
    <h1>Ententendo e comprenendedo a tag slot</h1>
    <template v-slot:title>
      delta 2730
    </template>
    <template v-slot:person>
      <p>Desse modo, podemos trbalhar no compoente pai como se fose um html comum, onde o componete filho terá um dos tipos de slots deixando o seu codigo mais dinamico possivel</p>
    </template>
  </Info>
</template>

<script>
import Info from './info.vue';
export default {
  name: 'Aula',
  data(){
    return {
      aula: "Slots"
    }
  },
  components: {
    Info
  }
}
</script>