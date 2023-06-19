<template>
    <!-- <h2>Aula - 22</h2> -->
    <div>
        <slot></slot>
        <slot name='title'></slot>
        <p>A tag <strong>slot</strong> pode ser usada para deixar o seu codigo mais fluido e flexivel;</p>
        <p>Ela pode se declarada em um dos componentes, para isso ela é dividida de duas formas declarativas;</p>
        <li>Modo padrão: <strong>slot</strong></li>
        <li>Modo especifico: <strong>slot name=""</strong></li>
        <h2>
            <slot name="person"></slot>
        </h2>
    </div> 
</template>

<script>
export default {
    name: "Info",
    mounted(){
        console.log(this.$slots);
    }
}
</script>