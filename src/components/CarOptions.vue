<template>
    <h2>Coche-Options API</h2>
    
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencia: {{ power }}</p>
    <button @click="upPower(50)">Aumentar</button>
    <button @click="downPower">Disminuir</button>

    

    
</template>

<script lang="ts">
export default {
    data() {
        return {
            brand: "Seat",
            model: "Leon",
            color: ["Azul", "Rojo", "Verde"],
            power: 50,
            price: 38000,
             mensaje: {
                title: "Hola mundo",
                text: "Adios",
           },
         };
       },
       methods: {
        upPower(newPower) {
            this.power = this.power + newPower;
        },
        downPower() {
            this.power --;

        }
       }
    }


</script>

<style>

</style>