<template>
  <a-layout>
    <ALayoutHeader>
      <Container>
        <div class="nav-container">
          <div class="left-content">
            <img src="../assets/icons/camera.png" alt="" width="25px" />
            <RouterLink to="/" style="font-size: 18px">Snaptrail</RouterLink>
            <AInputSearch
              v-model:value="searchUser"
              style="width: 300px"
              placeholder="input search text"
              @search="onSearch"
            />
          </div>
          <div v-if="!isAuthenticated" class="right-content">
            <AuthModal :isLogin="false" />
            <AuthModal :isLogin="true" />
          </div>
          <div v-else class="right-content">
            <AButton type="primary">My Profile</AButton>
            <AButton type="primary">Logout</AButton>
          </div>
        </div>
      </Container>
    </ALayoutHeader>
  </a-layout>
</template>

<script setup>
import { RouterLink } from "vue-router";
import Container from "./Container.vue";
import AuthModal from "./AuthModal.vue";
import { ref } from "vue";

const searchUser = ref("");
const isAuthenticated = ref(true);

const onSearch = () => {};
</script>

<style scoped>
.nav-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.left-content {
  display: flex;
  align-items: center;
}
.left-content a {
  margin-left: 10px;
  margin-right: 20px;
}

.right-content {
  display: flex;
  align-items: center;
}

.right-content > * {
  margin-left: 10px;
}
</style>
