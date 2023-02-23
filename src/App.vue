<script setup lang="ts">
import uiInput from './components/ui/ui-input.vue';
import uiCheckbox from './components/ui/ui-checkbox.vue';
</script>

<template>
  <div class="list">
    <ui-input placeholder="Text input" />
    <ui-checkbox />
  </div>
</template>

<style scoped>
.list {
  display: grid;
  grid-template-columns: 1fr;
  grid-row-gap: 32px;
  width: 320px;
  margin: 0 auto;
  padding: 40px 0 0;
}

.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
