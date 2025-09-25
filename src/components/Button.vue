<script setup></script>
<template>
  <button class="button">
    <div>
      <slot name="icon"></slot>
      <div>
        <slot name="txt"></slot>
      </div>
    </div>
    <slot> </slot>
  </button>
</template>

<style scoped>
.button {
  border: none;
  border-radius: 5px;
  background: var(--gradient);
  padding: 14px;
  font-family: var(--fond);
  font-size: 20px;
  font-weight: 600;
  color: var(--color-primary);
  cursor: pointer;
}
.button:hover {
  background: var(--gradient-inverted);
}
</style>
