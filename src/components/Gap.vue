<template>
  <div class="gap"><slot></slot></div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Gap',
  props: {},
});
</script>

<style scoped>
.gap {
    display: flex;
    gap: 10px;
}
</style>
