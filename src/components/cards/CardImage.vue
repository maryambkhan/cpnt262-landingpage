<template>
<div class="flex justify-center">
  <img
    :src="props.url"
    :alt="props.alt"
    class=" mt-6 ml-2 w-3/5 h-3/5"
  />
</div>
</template>
<script setup>
  const props = defineProps({
    url: {
      type: String,
      required: true,
    },
    alt: {
      type: String,
    },
  });
</script>