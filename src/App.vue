<template>
  <h1>Buttons</h1>

  <Gap>
    <Button>
      Default button
    </Button>

    <Button :transparent="true">
      Button with out background
    </Button>
  </Gap>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Button from './components/Button.vue';
import Gap from './components/Gap.vue';

export default defineComponent({
  name: 'App',
  components: {
    Button,
    Gap
  }
});
</script>

<style>
#app {
  font-family: sans-serif;
}
</style>