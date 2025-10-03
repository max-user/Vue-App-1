<script setup>
import Stat from "./components/Stat.vue";
import SitySelect from "./components/SitySelect.vue";

const data = {
  lable: "Влажность",
  stat: "90%",
};
const data2 = {
  lable: "Осадки",
  stat: "0%",
};

function getCity(city) {
  console.log(city);
}
</script>

<template>
  <main class="main">
    <Stat :lable="data.lable" v-bind:stat="data.stat"></Stat>
    <Stat v-bind="data2"></Stat>
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
