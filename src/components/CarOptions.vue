<template>
    <h2>Coche-Options API</h2>
    
    <p>Marca: {{ brand }}</p>
    <p>Modelo: {{ model }}</p>
    <p>Potencias Urbanas menor a 300 cv</p>
    <ul>
        <template v-for="(power, index) in powers" :key="index">
          
            <li v-if="power < 280">Urbana: {{ power }}</li>
            <li v-else-if="power === 280"> Hibrido: {{ power }}</li>
            <li v-else> Carrera: {{ power }}</li>

            <li v-if="power === 500">Super: {{ power }}</li>

        </template>
    </ul>

    
</template>

<script lang="ts">
export default {
//    data() {
//     return {
//         brand: "Audi",
//         model: "A4",
//         color: ["Azul", "Rojo", "Verde"],
//         power: 100,
//         price: 38000,
//         mensaje: {
//             title: "Hola mundo",
//             text: "Adios",
//         },
//     };
//    },
setup() {
    const brand = "Audi";
    const model = "A4";
    const powers = [60, 80, 120, 160, 200, 280, 300, 390, 540, 500];
    
    return {
        brand,
        model,
        powers,
        
    };
},
};
</script>

<style>

</style>