<template>
  <div>
    <p>Count: {{ count }}</p>
    <button @click="increment">Increment</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

// 반응형 상태 정의
const count = ref(0)

// 메서드 정의
const increment = () => {
  count.value++
}
</script>

<style scoped>
p {
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}
button {
  background-color: #42b883;
  color: white;
  border: none;
  border-radius: 6px;
  padding: 0.5rem 1rem;
  cursor: pointer;
  transition: background-color 0.2s;
}
button:hover {
  background-color: #2c9c6b;
}
</style>
