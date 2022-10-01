<script setup lang="ts">
import ChildComponent from './components/ChildComponentWithGenerics.vue'

const getSomeStrings = () => ["foo", "bar"]
</script>

<template>
  <div>
    <child-component
      :prop-one="5"
      :prop-two="getSomeStrings"
    />
  
    <child-component
      prop-one="vite rocks!"
      :prop-two="getSomeStrings"
    />
  </div>
</template>