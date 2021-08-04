<template>
  <button :class="{'button-transparent': transparent}" class="button">
    <slot></slot>
  </button>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Button',
  props: {
    transparent: Boolean
  },
});
</script>

<style scoped>
.button {
  font: inherit;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  background-color: #AD5CAD;
  color: #fff;
  border: 2px solid #AD5CAD;
  border-radius: 7px;
  padding: 8px 20px;
  transition: 0.3s;
  cursor: pointer;
}

.button:hover {
  opacity: 0.9;
}

.button:active {
  background-color: #b149b1;
}

.button-transparent {
  background-color: transparent;
  color: #AD5CAD;
}

.button-transparent:active {
  background-color: transparent;
  color: #b149b1;
  border-color: #b149b1;
}
</style>
