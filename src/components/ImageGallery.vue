<template>
  <div class="image-gallery-container">
    <img
      v-for="post in posts"
      :key="post.id"
      :src="post.imageUrl"
      alt="user-post-image"
    />
  </div>
</template>
<script setup>
const props = defineProps(["posts"]);
</script>

<style scoped>
.image-gallery-container {
  display: flex;
  justify-content: left;
  flex-wrap: wrap;
  gap: 10px;
  padding: 0 75px;
}

img {
  margin: 5px;
  width: 200px;
}
</style>
