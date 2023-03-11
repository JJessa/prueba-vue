
<template>
 <h1>Hola vue JS</h1>
<CarComposition />
<CarOptions />


</template>

<script>
import CarComposition from "./components/CarComposition.vue";
import CarOptions from "./components/CarOptions.vue";
export default {
  components: {
    CarComposition,
    CarOptions,
  }
}
</script>

<style>
h1 {
  color: red;
}
</style>


