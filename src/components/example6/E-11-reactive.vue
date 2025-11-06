<template>
  <div>
    <p>Name: {{ person.name }}</p>
    <p>Age: {{ person.age }}</p>
    <button @click="incrementAge">Increment Age</button>
  </div>
</template>

<script setup>
import { reactive } from 'vue'

// reactive로 객체 상태 정의
const person = reactive({
  name: 'John Doe',
  age: 30
})

// 메서드 정의
const incrementAge = () => {
  person.age++
}
</script>

<style scoped>
p {
  font-size: 1.2rem;
  margin: 0.3rem 0;
}

button {
  background-color: #42b883;
  color: white;
  border: none;
  border-radius: 6px;
  padding: 0.4rem 1rem;
  cursor: pointer;
  transition: background-color 0.2s;
}

button:hover {
  background-color: #2c9c6b;
}
</style>
