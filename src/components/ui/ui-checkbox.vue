<script setup lang="ts"></script>

<template>
  <label>
    <input class="input-checkbox" id="c1" type="checkbox" />
    <span class="input-checkbox-pseudo" />
  </label>
</template>

<style>
:root {
  --background-color: #fff;
  --border-color: #e1e6f9;
  --focus-color: transparent;
}

.input-checkbox {
  position: absolute;
  -webkit-appearance: none;
  -moz-appearance: none;
}

.input-checkbox-pseudo {
  display: block;
  width: 22px;
  height: 22px;
  border: 1px solid var(--border-color);
  border-radius: 6px;
  box-shadow: inset 0 0 0 1px var(--border-color), 0 0 0 3px var(--focus-color);
  background-color: var(--background-color);
  cursor: pointer;

  transition: background 0.3s, border-color 0.3s, box-shadow 0.2s;
}

.input-checkbox:focus + .input-checkbox-pseudo {
  --focus-color: #eceffc;
}

.input-checkbox:focus + .input-checkbox-pseudo,
.input-checkbox-pseudo:hover {
  --border-color: #bbc1e1;
}

.input-checkbox:checked + .input-checkbox-pseudo {
  --background-color: #bbc1e1;
  --border-color: #bbc1e1;
}
</style>
