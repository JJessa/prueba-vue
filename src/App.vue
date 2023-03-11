
<template>
 <h1>Hola vue JS
<CarOptions />
<hr/>
<CarComposition />
</h1>


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
  font-size: 1.2rem;
}
</style>


