<template>
  <Container>
    <div class="profile-container">
      <Userbar
        username="Weeeknd"
        :userInfo="{ post: 4, follower: 400, following: 8000 }"
      />
      <ImageGallery
        :posts="[
          {
            id: 1,
            imageUrl:
              'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdJKncgYFP-O8CwJz4o989Jx1TzcWf82CkRw&s',
          },
          {
            id: 2,
            imageUrl:
              'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdJKncgYFP-O8CwJz4o989Jx1TzcWf82CkRw&s',
          },
          {
            id: 3,
            imageUrl:
              'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdJKncgYFP-O8CwJz4o989Jx1TzcWf82CkRw&s',
          },
          {
            id: 4,
            imageUrl:
              'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdJKncgYFP-O8CwJz4o989Jx1TzcWf82CkRw&s',
          },
          {
            id: 5,
            imageUrl:
              'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdJKncgYFP-O8CwJz4o989Jx1TzcWf82CkRw&s',
          },
          {
            id: 6,
            imageUrl:
              'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdJKncgYFP-O8CwJz4o989Jx1TzcWf82CkRw&s',
          },
        ]"
      />
    </div>
  </Container>
</template>
<script setup>
import Container from "./Container.vue";
import ImageGallery from "./ImageGallery.vue";
import Userbar from "./Userbar.vue";
</script>

<style scoped>
.profile-container {
  display: flex;
  flex-direction: column;
  padding: 20px 0;
}
</style>
