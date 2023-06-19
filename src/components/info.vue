<template>
    <!-- <h2>Aula - 21</h2> -->
    <div>
        <p>Sendo declarado na parte <strong>script</strong>, o <strong>watch</strong> é um objeto que obsevará um
            determinado valor e executará uma determinada função;</p>
        <p>tendo semelhança com os ganchos de ciclo de vida (Life cycle hooks);</p>
        <p>No entanto para que funcione, é nescessario term uma função com o mesmo nome da variavel que deseja observar,
            retornando dois parametros, <strong>NewValue & OldValue</strong></p>

        <p>Os observadores profundos, caso vc mexa com um componente mais interno como <strong>user.lName</strong>, vc deve transformar o watcher um objeto;</p>
        
        <p>Os observadores profundos, deixam duas funcioladades visiveis o <strong>handler()</strong>, que é o que vai executar, uma função qualquer. E um <strong>deep(profrundo)</strong> que deve retornar um booleano, que quando qualquer coisa no objeto mudar, exute o handler()</p>

        <input type="text" placeholder="primeiro nome" v-model="user.fName"><br>
        <input type="text" placeholder="sobrenome" v-model="user.lName">
        <br>
        <select v-model="pageCount">
            <option value="0" disabled>0</option>
            <option value="5">5</option>
            <option value="10">10</option>
            <option value="15">15</option>
        </select> <br>
        <img :src="url" alt="pokemon">
    </div>
</template>

<script>
export default {
    name: "Info",
    data() {
        return {
            pageCount: '0',
            user: {
                fName: '',
                lName: ''
            },
            url: ''
        }
    },
    watch: {
        pageCount(nv) {
            if (nv >= 5) {
                this.savePage()
            }
        },
        user: {
            handler(){
                console.log('Tudo ok');
            },
            deep: true
        }
    },
    methods: {
        async savePage() {
           console.log('merda');
           this.url = `https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/${this.pageCount}.png`
        }
    }
}
</script>