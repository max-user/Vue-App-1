<script setup></script>
<template>
  <button class="button">
    <slot> </slot>
  </button>
</template>

<style scoped>
.button {
  border: none;
  border-radius: 50px;
  font-size: 24px;
  padding: 14px;
  background: var(--color-bg-button-dz);
  color: var(--color-primary);
}
</style>
