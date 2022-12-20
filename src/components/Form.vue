<template>
    <!-- <h2>Aula - 08</h2> -->
    <form action="">
        <div>
            <InputTxT/>
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
    export default {
        name: 'Form',
        components: {
            InputTxT,
            BtnSubmi,
        },
        data(){

        }
    }
</script>