<script setup lang="ts">
import { useCounterStore } from '@/stores/modules/count'

const counter = useCounterStore()
const increment = () => {
  counter.count++
}
</script>
<template>
  <view>Current Count: {{ counter.count }}</view>
  <button @click="increment">add count</button>
</template>
