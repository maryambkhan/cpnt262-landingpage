<template>
    <h1 class="flex justify-center font-semibold text-red-900">{{props.title}}</h1>
</template>

<script setup>
import { defineProps } from "vue";
const props = defineProps({
  title: {
    type: String,
  },
});
</script>