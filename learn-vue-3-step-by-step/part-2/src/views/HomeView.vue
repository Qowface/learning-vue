<script setup>
import QuizComponent from '@/components/Quiz/QuizComponent.vue'
</script>

<template>
  <main>
    <QuizComponent :quiz="{ name: 'My First Quiz', questions: [] }" />
  </main>
</template>
