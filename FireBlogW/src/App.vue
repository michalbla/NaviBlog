<script>
import { RouterView } from "vue-router";
import Navigation from "@/components/Navigation.vue";
export default {
  components: {
    Navigation,
  },
};
</script>

<template>
  <header class="flex p-6 items-center">
    <div class="logo pt-2">
      <RouterLink :to="{ path: '/' }">
        <img src="./assets/icons/logo.svg" alt="" />
      </RouterLink>
    </div>
    <Navigation />
  </header>

  <RouterView />
</template>

<style>
</style>
