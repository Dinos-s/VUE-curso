<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <Aula/>
  </div>
</template>

<script>
// @ is an alias to /src
import Aula from '@/components/Aula.vue'

export default {
  name: 'HomeView',
  components: {
    Aula
  }
}
</script>
