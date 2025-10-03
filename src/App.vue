<script setup>
import Stat from "./components/Stat.vue";
import SitySelect from "./components/SitySelect.vue";

const data = {
  label: "Влажность",
  stat: "90%",
};

function getCity(city) {
  console.log(city);
}
</script>

<template>
  <main class="main">
    <Stat v-bind="data"></Stat>
    <Stat v-bind:label="'Осадки'" v-bind:stat="'10%'"></Stat>
    <SitySelect @select-city="getCity" />
  </main>
</template>

<style scoped>
.main {
  background: var(--color-bg-main);
  padding: 50px;
  border-radius: 25px;
}
</style>
