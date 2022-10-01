<script setup lang="ts">
defineProps<MyChildProps<unknown>>()
</script>

<script lang="ts">
export interface MyChildProps<T> {
  propOne: T
  propTwo: () => Array<T>
}
</script>

<template>
  <div>{{ propOne }}</div>
</template>