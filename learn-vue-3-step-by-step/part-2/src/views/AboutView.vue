<script>
import flash from '@/mixins/flash'

export default {
  mixins: [flash]
}
</script>

<template>
  <div>
    <button @click="flash('It Works On The About Page!')">Click Me</button>
  </div>
</template>
