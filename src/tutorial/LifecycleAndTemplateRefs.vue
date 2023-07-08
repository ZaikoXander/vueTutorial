<script setup lang="ts">
import { Ref, onMounted, onUnmounted, ref } from 'vue'

  const pElementRef: Ref<HTMLParagraphElement | null> = ref<HTMLParagraphElement | null>(null)

  onMounted(() => {
    (pElementRef.value as HTMLParagraphElement).textContent = "hello world"
  })

  onUnmounted(() => {
    console.log("Don't do that! What is your problem?!??")
  })
</script>

<template>
  <p ref="pElementRef">hello</p>
</template>
