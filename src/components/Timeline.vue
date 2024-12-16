<template>
  <Container>
    <div class="timeline-container">
      <Card v-for="post in data" :key="post.id" :post="post" />
    </div>
  </Container>
</template>
<script setup>
import Card from "./Card.vue";
import Container from "./Container.vue";

const data = [
  {
    id: 1,
    username: "Divyansh",
    url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRPaG-hKNIgvedxbVF_ap-S4oOkXcNGMhagKQ&shttps://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRPaG-hKNIgvedxbVF_ap-S4oOkXcNGMhagKQ&s",
    caption: "Hello Guys",
  },
  {
    id: 2,
    username: "Saurabh",
    url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdJKncgYFP-O8CwJz4o989Jx1TzcWf82CkRw&s",
    caption: "namaste",
  },
  {
    id: 3,
    username: "Gelid",
    url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4M20QhML8edk6mdLSG3WGnIQH07W9HRUqGw&s",
    caption: "Hello Guys",
  },
  {
    id: 4,
    username: "Zen",
    url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRXJA32WU4rBpx7maglqeEtt3ot1tPIRWptxA&s",
    caption: "Hello Guys",
  },
  {
    id: 5,
    username: "Geralt",
    url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRPaG-hKNIgvedxbVF_ap-S4oOkXcNGMhagKQ&shttps://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRPaG-hKNIgvedxbVF_ap-S4oOkXcNGMhagKQ&s",
    caption: "hmmm",
  },
  {
    id: 6,
    username: "Ichigo",
    url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4M20QhML8edk6mdLSG3WGnIQH07W9HRUqGw&shttps://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4M20QhML8edk6mdLSG3WGnIQH07W9HRUqGw&s",
    caption: "Hello Guys",
  },
  {
    id: 7,
    username: "Sung jin woo",
    url: "https://images.pexels.com/photos/3680219/pexels-photo-3680219.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500",
    caption: "",
  },
];
</script>

<style scoped>
.timeline-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px 0;
}
</style>
