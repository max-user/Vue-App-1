<script setup>
import { ref } from "vue";
import Button from "./Button.vue";
import iconLocation from "../icon/iconLocation.vue";

let isEdited = ref(false);

const emit = defineEmits({
  selectCity(payload) {
    return payload;
  },
});

function select() {
  isEdited.value = false;
}
function edit() {
  isEdited.value = true;
}
</script>
<template>
  {{ isEdited }}
  <Button @click="edit()"> <iconLocation /> Изменить город </Button>
  <input type="button" value="Вася" />
  <Button @click="select()"> Сохранить </Button>
</template>
<style scoped></style>
