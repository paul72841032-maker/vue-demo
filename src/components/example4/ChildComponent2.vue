<template>
  <div>
    <p>{{ sharedMessage }}</p>
  </div>
</template>

<script setup>
import { inject } from 'vue'

// 부모 컴포넌트에서 제공(provide)한 데이터 주입
const sharedMessage = inject('sharedMessage')
</script>

<style scoped>
p {
  font-size: 1.5rem;
}
</style>
