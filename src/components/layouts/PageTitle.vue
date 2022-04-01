<template>
    <h1 class="flex justify-center font-semibold text-4xl mt-8">{{props.title}}</h1>
    </template>

    <script setup>
const props = defineProps({
  title: {
    type: String,
    default:'Heading'
  }
  });
</script>