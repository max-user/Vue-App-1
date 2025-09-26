<script setup>
const d = new Date();
</script>

<template>
  Date: {{ d.getDate() }} - {{ d.getMonth() }} - {{ d.getFullYear() }}
</template>

<style scoped></style>
