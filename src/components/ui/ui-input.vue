<script setup lang="ts"></script>

<template>
  <input class="input" />
</template>

<style>
:root {
  --background-color: #fff;
  --border-color: #e1e6f9;
  --focus-color: transparent;
}
.input {
  display: block;
  padding: 0 20px;
  height: 48px;

  border: none;
  border-radius: 12px;
  outline: none;
  background-color: var(-background-color);

  transition: box-shadow 0.25s;
  box-shadow: inset 0 0 0 1px var(--border-color), 0 0 0 3px var(--focus-color);

  transition: background 0.3s, border-color 0.3s, box-shadow 0.2s;
}

.input:focus {
  --focus-color: #eceffc;
}

.input:focus,
.input:hover {
  --border-color: #bbc1e1;
}
</style>
