<template>
  <header class="flex  justify-between bg-black py-4">
    <TheLogo />
    <div class="flex justify-center">
      <span class="text-2xl font-semibold text-white">SEPHORA</span> 
    </div>
   <TheNavBar />
  </header>
</template>

<script setup>
import TheNavBar from "./TheNavBar.vue";
import TheLogo from "./TheLogo.vue";
</script>