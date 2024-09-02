<script setup>
import QuizComponent from '@/components/Quiz/QuizComponent.vue'
import { state } from '@/stores/quizStore'
</script>

<template>
  <main>
    <QuizComponent :quiz="state" />
  </main>
</template>
