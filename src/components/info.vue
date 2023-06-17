<template>
    <!-- <h2>Aula - 19</h2> -->
    <p>Assim como já foi visto anteriomente, o <strong>v-bind / ':'</strong> que é utilizado para elementos e atributos
        dinamicos, ele tbm pode ser usado com os estilos.</p>
    <p :class="[novaClasse]">Tambem podemos utilizar listas de itens '['']', de objetos '[{}]', ou até  mesmo um objeto {}</p>
    <p :class="['text']">Nas lista temos a possibilidade de abrigar mais de uma classe</p>
    <p :class="{'tudoCerto': isOk}">Com os objeto devem ser atibuidos com valore bolleanos(true/false)</p>
    
    <button :class="multiClass" @click="mudaCor" type="button">Teste aqui!</button>
</template>

<script>
export default {
    name: "Info",
    data() {
        return {
            btnText: 'Teste aqui!',
            active: true,
            isOk: true,
            multiClass: ['text', 'tudoCerto']
        }
    },
    methods: {
        mudaCor(){
            this.active = !this.active
        }
    },
    computed: {
        novaClasse() {
            return {
                test: this.active,
                test2: !this.active
            }
        }
    }
}
</script>

<style>
.test {
    font-size: 12px;
    color: red;
}

.test2 {
    background-color: aqua;
    color: black;
}

.tudoCerto {
    background-color: rgb(50, 115, 168);
}

.text{
    font-style: italic;
}
</style>