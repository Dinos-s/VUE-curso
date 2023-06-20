<template>
  <div class="about">
    <h1>This is an about page</h1>
    <h2>Aula 23 - Rotas</h2>
    <Info/>
  </div>
</template>

<script>
import Info from '@/components/info.vue';
export default {
    name: "about",
    components: {
      Info 
    }
}
</script>