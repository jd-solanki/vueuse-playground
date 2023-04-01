<script setup lang="ts">
import { resolveRef } from '@vueuse/core';
import { ref } from 'vue';

const foo = ref('hi')

const a = resolveRef(0) // Ref<number>
const b = resolveRef(foo) // Ref<string>
const c = resolveRef(() => 'hi') // ComputedRef<string>
</script>

<template>
  <main>
    <p>Welcome!</p>
  </main>
</template>
