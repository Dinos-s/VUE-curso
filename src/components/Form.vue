<template>
    <form action="" @submit="enviar_Form($event)">
        <div>
            <input type="text" v-model="name">
        </div>
        <div>
            <InputTxT/>
        </div>
        <div>
            <BtnSubmi/>
        </div>
    </form>
</template>

<script>
    import InputTxT from "./form/InputText.vue";
    import BtnSubmi from "./form/submit.vue";
    export default{
        name: 'Form',
        components:{
            InputTxT,
            BtnSubmi,
        },
        data(){
            // dados do formulário
            return{
                name: '',
            }
        },
        methods:{
            enviar_Form(e){
                
                e.preventDefault(); //pausa a subimisão dos dados a serem enviados

                const name = this.name
                console.log('Form envido');
                console.log(`nome: ${name}`);
            }
        }
    }
</script>