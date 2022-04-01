<template>
    <h1 class="flex justify-end pr-20 mr-20 text-blue-900 hover:underline">{{props.title}}</h1>
    </template>

    <script setup>
const props = defineProps({
  title: {
    type: String,
    default:'Heading'
  }
  });
</script>