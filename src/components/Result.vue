<script setup>
import { defineProps } from "vue";
import { RouterLink } from "vue-router";

const { correctAnswers, quizQuestionLength } = defineProps([
  "correctAnswers",
  "quizQuestionLength",
]);
</script>
<template>
  <div class="results">
    <p>Your Results</p>
    <h1>{{ correctAnswers }}/{{ quizQuestionLength }}</h1>
    <RouterLink to="/">Home</RouterLink>
  </div>
</template>
<style scoped>
.results {
  text-align: center;
  padding: 100px 0;
}

p {
  font-size: 25px;
}
</style>
