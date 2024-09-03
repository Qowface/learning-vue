<script setup>
import { useFlash } from '@/composables/useFlash'
import { useCounterStore } from '@/stores/CounterStore'

let { flash } = useFlash()
let counter = useCounterStore()
</script>

<template>
  <p>About Page. The current count is {{ counter.count }}</p>
  <div>
    <button @click="flash('Yay!', 'It Works On The About Page!', 'info')">Click Me</button>
  </div>
</template>
