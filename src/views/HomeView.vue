<script setup lang="ts">
import { useMounted } from '@vueuse/core';

const isMounted = useMounted()
</script>

<template>
  <main>
    <p>Is mounted: {{ isMounted }}</p>
  </main>
</template>
