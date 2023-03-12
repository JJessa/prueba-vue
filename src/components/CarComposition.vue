
<template>
    <h2>Coche - Composition API</h2>
    
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencia: {{ power }}</p>
    <button @click="upPower(20)">Aumentar</button>
    <button @click="downPower(10)">Disminuir</button>
   

    
</template>

<script>
import { ref } from "vue";
export default {
setup() {
    const brand = "Audi";
    const model = "A4";
    let power = ref(40);

    const upPower = (newPower) => {
        console.log("Aumentando potencia...");
        power.value = power.value + newPower;
    };
    const downPower = (newPower) => {
        console.log("Disminuyendo potencia... " + newPower);
        power.value = power.value - newPower;

    }
    
    return {
        brand,
        model,
        power,
        upPower,
        downPower,
        
    };
},
};
</script>

<style>

</style>