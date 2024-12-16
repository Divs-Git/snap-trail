<template>
  <div class="userbar-container">
    <div class="user-name-header">
      <ATypographyTitle :level="2">{{ username }}</ATypographyTitle>
    </div>
    <div class="user-info-container">
      <ATypographyTitle :level="5">{{ userInfo.post }} posts</ATypographyTitle>
      <ATypographyTitle :level="5"
        >{{ userInfo.follower }} followers</ATypographyTitle
      >
      <ATypographyTitle :level="5"
        >{{ userInfo.following }} following</ATypographyTitle
      >
    </div>
  </div>
</template>

<script setup>
const props = defineProps(["username", "userInfo"]);
</script>

<style scoped>
.userbar-container {
  padding: 20px 75px;
  margin-bottom: 45px;
}

.user-info-container {
  display: flex;
  align-items: center;
}

.user-info-container h5 {
  margin: 0;
  padding: 0;
  margin-right: 30px;
}
</style>
