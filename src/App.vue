<template>
  <h1>Buttons</h1>

  <div class="gap">
    <Button>
      Default button
    </Button>

    <Button :transparent="true">
      Button with out background
    </Button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Button from './components/Button.vue';

export default defineComponent({
  name: 'App',
  components: {
    Button
  }
});
</script>

<style>
#app {
  font-family: sans-serif;
}

.gap {
  display: flex;
  gap: 10px;
}
</style>