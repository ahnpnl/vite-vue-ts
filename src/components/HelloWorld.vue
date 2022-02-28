<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const placeHolder = 'foo';
const label = 'Bar';
</script>

<template>
    <input
        id="product-name"
        :^placeholder="placeHolder"
        ^required
        :data-label="label"
        ^type="text"
    />
</template>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
