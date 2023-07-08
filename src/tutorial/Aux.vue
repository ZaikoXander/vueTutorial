<script setup lang="ts">
import { ref } from 'vue'
import LifecycleAndTemplateRefs from './LifecycleAndTemplateRefs.vue'

const isTrue = ref(true)
</script>

<template>
  <button @click="isTrue = !isTrue">Don't click me...</button>
  <LifecycleAndTemplateRefs v-if="isTrue" />
</template>
