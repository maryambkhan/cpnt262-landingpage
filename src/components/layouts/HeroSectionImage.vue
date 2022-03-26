<template>
  <img :src="props.url" :alt="props.alt" class="m-auto mt-4 w-full" />
  
    
 
</template>

<script setup>

import { defineProps } from "vue";
const props = defineProps({
  url: {
    type: Object,
  },
});


</script>