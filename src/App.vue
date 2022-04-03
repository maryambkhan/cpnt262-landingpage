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
    <section class="flex justify-end mt-4 bg-gray-200 p-2">
       <p class="mr-2">Message is: {{ message }}</p>
      <input  :v-model="text" :v-on="message"
        class="
          mr-2
          placeholder:italic placeholder:text-slate-400
          block
          bg-white
          border border-slate-800
          rounded-md
          py-2
          pl-9
          pr-3
          shadow-sm
          focus:outline-none
          focus:border-sky-500
          focus:ring-sky-500
          focus:ring-1
          sm:text-sm
        "
        placeholder="Search"
        type="text"
        name="search"
      />
    </section>
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
    <ThePostCard />
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

import { ref } from 'vue'
import TheHeader from "./components/ui/TheHeader.vue";
import HeroSection from "./components/layouts/HeroSection.vue";
import TheFooter from "./components/ui/TheFooter.vue";
import CardImage from "./components/cards/CardImage.vue";
import CardInfo from "./components/cards/CardInfo.vue";
import ActionButton from "./components/utilities/ActionButton.vue";
import CardLayout from "./components/cards/CardLayout.vue";
import CardTitle from "./components/cards/CardTitle.vue";
import PageTitle from "./components/layouts/PageTitle.vue";
import PostLayout from "./components/posts/PostLayout.vue";
import Postcard from "./components/posts/PostCard.vue";
import ThePostCard from "./components/posts/posts-1/ThePostCard.vue";

const cards = [
  // first card
  {
    title: "Blush",
    info: "Lorem Ipsum is simply dummy text ",
    image: require(`./assets/images/blush.jpeg`),
  },

  // second card

  {
    title: "Combo",
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
    title: "Perfume",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/perfume.jpeg`),
  },

  // six card
  {
    title: "Lip Gloss",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/gloss.jpeg`),
  },

  // seven card
  {
    title: "Highlighter",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/highlighter.jpeg`),
  },

  // eight card
  {
    title: "Brushes",
    info: "Lorem Ipsum iss simply dummy text",
    image: require(`./assets/images/brushes.jpeg`),
  },
];

function onChange (message){
  console.log (message);
}
</script>

