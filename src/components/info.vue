<template>
    <!-- <h2>Aula - 23</h2> -->
    <div>
        <p>o vue router, por padrão não vem no projeto inicializado no vue cli(caso ñ tenha escolhido o pluguin), para
            instalar esse pluguis use o npm i vue-router</p>

        <p>ou use o vue add router e marque não na pergunta, já que ele sobreescreve alguns arquivos no projeto que é
            instalado;</p>

        <p>Caso vc tenha inicializado o router com npm, vc deve criar uma pasta para rotas em js, e uma pasta para o
            arquivos de views com vue, e no main.js import o router;</p>

        <p>na pasta router, no index.js, algumas estruturas basicas, percerba que a constante rotas retorna um array de objetos e no objeto about, temos uma info extra:</p>
        <li>component: () => import('../views/about.vue')</li>
        <p>a parti desse ponto é nescessário entender que essa rota só será carregada caso seja executada;</p>
    </div>
</template>

<script>
export default {
    name: "Info",
}
</script>