<script setup>
import { useFlash } from '@/composables/useFlash'

let { flash } = useFlash()
</script>

<template>
  <div>
    <button @click="flash('Yay!', 'It Works On The About Page!', 'info')">Click Me</button>
  </div>
</template>
