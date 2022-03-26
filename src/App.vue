<template>
  <TheHeader />
  <main>
    <div>
      <HeroSectionImage />
    </div>
  </main>
  <TheFooter :title="'&copy; Maryam Khan 2022'" />
</template>

<script setup>
import TheHeader from "./components/ui/TheHeader.vue";
import HeroSectionImage from "./components/layouts/HeroSection.vue";
import TheFooter from "./components/ui/TheFooter.vue";
</script>