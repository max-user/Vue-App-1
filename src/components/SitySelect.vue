<script setup>
import Button from "./Button.vue";
import iconLocation from "../icon/iconLocation.vue";

const emit = defineEmits({
  selectCity(payload) {
    return payload;
  },
});
function select() {
  emit("selectCity", "London");
}
</script>
<template>
  <Button @click="select()"> <iconLocation /> Изменить город </Button>
  <input type="button" value="Вася" />
  <Button> Сохранить </Button>
</template>
<style scoped></style>
