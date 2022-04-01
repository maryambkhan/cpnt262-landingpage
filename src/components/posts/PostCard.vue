<template>
  <div>
    <article
      class="
        backgroundImage
        grid
        text-center
        content-center
        mt-4
				m-auto

      "
    >
      <PostCardTitle />
      <PostCardText />
    </article>
  </div>
</template>
<script setup>
import PostCardTitle from "./PostCardTitle.vue";
import PostCardText from "./PostCardText.vue";
</script>

<style scoped>
.backgroundImage {
  height: 80vh;
  min-width: 50vw;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-image: url(../../assets/images/blackposter.jpeg);
}
</style>