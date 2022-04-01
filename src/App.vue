<template>
  <!--The header-->
  <TheHeader />
  <!--Main Section-->
  <main>
    <!--Hero Section-->
    <div>
      <HeroSection />
    </div>
    <!-- Card Section-->
    <PageTitle :title="'Brand-New Additions'" />
    <PageAction :title="'Show More'" />
    <section>
      <div class="flex flex-wrap justify-center mt-8">
        <card-layout v-for="card in cards" :key="card.id">
          <card-image :url="card.image" />
          <card-title>{{ card.title }}</card-title>
          <card-info>{{ card.info }}</card-info>
          <action-button>Add to Cart</action-button>
        </card-layout>
      </div>
    </section>
    <!--Post Card Section-->
    <Postcard />
    <!--cards-->
    <PageTitle :title="'Selling Fast'" />
    <section>
      <div class="flex flex-wrap justify-center mt-8">
        <card-layout v-for="card in cards" :key="card.id">
          <card-image :url="card.image" />
          <card-title>{{ card.title }}</card-title>
          <card-info>{{ card.info }}</card-info>
          <action-button>Add to Cart</action-button>
        </card-layout>
      </div>
    </section>
    <ThePostCard/>
     <section>
      <div class="flex flex-wrap justify-center mt-8">
        <card-layout v-for="card in cards" :key="card.id">
          <card-image :url="card.image" />
          <card-title>{{ card.title }}</card-title>
          <card-info>{{ card.info }}</card-info>
          <action-button>Add to Cart</action-button>
        </card-layout>
      </div>
    </section>
     <!--post-->
     <PostLayout />
  </main>
  <TheFooter :title="'&copy; Maryam Khan 2022'" />
</template>

<script setup>
import TheHeader from "./components/ui/TheHeader.vue";
import HeroSection from "./components/layouts/HeroSection.vue";
import TheFooter from "./components/ui/TheFooter.vue";
import CardImage from "./components/cards/CardImage.vue";
import CardInfo from "./components/cards/CardInfo.vue";
import ActionButton from "./components/utilities/ActionButton.vue";
import CardLayout from "./components/cards/CardLayout.vue";
import CardTitle from "./components/cards/CardTitle.vue";
import PageTitle from "./components/layouts/PageTitle.vue";
import PageAction from "./components/layouts/PageAction.vue";
import PostLayout from "./components/posts/PostLayout.vue";
import Postcard from "./components/posts/PostCard.vue";
import ThePostCard from "./components/posts/posts-1/ThePostCard.vue";

const cards = [
  // first card
  {
    title: "Lipstic",
    info: "Lorem Ipsum is simply dummy text ",
    image: require(`./assets/images/blush.jpeg`),
  },

  // second card

  {
    title: "Brushes",
    info: "Lorem Ipsum is simply dummy text ",
    image: require(`./assets/images/combo.jpeg`),
  },

  // third card
  {
    title: "EyeLiner",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/liner.jpeg`),
  },

  // fourth card
  {
    title: "Foundation",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/foundation.jpeg`),
  },
   
  // fifth card
  {
    title: "Foundation",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/perfume.jpeg`),
  },
  
  // six card
  {
    title: "Foundation",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/gloss.jpeg`),
  },
  
  // seven card
  {
    title: "EyeLiner",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/highlighter.jpeg`),
  },
  
  // eight card
  {
    title: "EyeLiner",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/brushes.jpeg`),
  },
];
</script>

