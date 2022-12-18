<template>
  <h1>Olá pessoas!</h1>
  <p>nome: {{ nome }}, trabalho no momento como {{ trabalho }}</p>
</template>

<script>
export default {
  name: 'firstComponent',
  data(){
    return {
      nome: "Gabriel",
      trabalho: "Jovem Aprendiz"
    }
  }
}
</script>