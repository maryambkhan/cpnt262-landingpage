<template>
  <TheHeader />
  <main>
  <div>
    <HeroSectionImage  :url="heroImage.backgroundImage"/>
    <HeroSectionTitle :title="heading" />
  </div>
 <TheFooter :title="'&copy; Maryam Khan 2022'" />
  </main>
</template>

<script setup>
import TheHeader from "./components/ui/TheHeader.vue";
import HeroSectionImage from "./components/layouts/HeroSectionImage.vue";
import TheFooter from "./components/ui/TheFooter.vue";
import HeroSectionTitle from "./components/layouts/HeroSectionTitle.vue";


// heroImage
const heroImage = {
  backgroundImage :"https://images.pexels.com/photos/2080960/pexels-photo-2080960.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260"
}

const heading ="Welcome to my page";
</script>