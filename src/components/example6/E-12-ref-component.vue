<template>
  <div>
    <input ref="inputField" type="text" placeholder="Click the button to focus" />
    <button @click="focusInput">Focus Input</button>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'

// DOM 요소 참조용 ref
const inputField = ref(null)

// 버튼 클릭 시 input에 포커스 주기
const focusInput = () => {
  inputField.value?.focus()
}

// 컴포넌트가 마운트될 때 자동 포커스
onMounted(() => {
  console.log(inputField) // 마운트 후 inputField 접근 가능
  inputField.value?.focus()
})
</script>

<style scoped>
div {
  display: flex;
  flex-direction: column;
  align-items: start;
  gap: 0.5rem;
}

input {
  padding: 0.4rem 0.8rem;
  border: 1px solid #ccc;
  border-radius: 6px;
  outline: none;
  transition: border-color 0.2s;
}

input:focus {
  border-color: #42b883;
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
