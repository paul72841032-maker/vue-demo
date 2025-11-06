<template>
  <div>
    <ChildComponent
        :message="parentMessage"
        @custom-event="handleEvent"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import ChildComponent from './ChildComponent.vue'

const parentMessage = ref('Hello from parent')

function handleEvent(payload) {
  console.log(payload) // 'Hello from child' 출력
}
</script>
