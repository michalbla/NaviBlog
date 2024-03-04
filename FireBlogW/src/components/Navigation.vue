<template>
  <nav class="navi">
    <div class="navi-menu">
      <RouterLink :to="{ path: '/' }" class="hover:text-lightOrange">O nas</RouterLink>
      <RouterLink :to="{ path: '/' }" class="hover:text-lightOrange">Kontakt</RouterLink>
      <RouterLink :to="{ path: '/' }" class="hover:text-lightOrange">Blog</RouterLink>
      <RouterLink :to="{ path: '/login' }" class="hover:text-lightOrange">Zaloguj</RouterLink>
    </div>
    <div class="navi-button">
      <RouterLink
        :to="{ path: '/' }"
        class="hidden md:block p-3 px-6 pt-2 text-white bg-lightOrange rounded-full baseline hover:bg-darkBlue">
        Zarejestruj</RouterLink>
    </div>
    <!-- <button id="menu-btn" class="block hamburger md:hidden focus:outline-none">
      <span class="hamburger-top"></span>
      <span class="hamburger-middle"></span>
      <span class="hamburger-bottom"></span>
    </button> -->
    <!-- <div class="md:hidden">
            <div id="menu" class="hidden absolute flex-col items-center self-end py-8 mt-10 space-y-6 font-bold bg-white sm:w-auto sm:self-center left-6 right-6 drop-shadow-md">
                <RouterLink :to="{ path: '/'}" class="hover:text-lightOrange">O nas</RouterLink>
                <RouterLink :to="{ path: '/'}" class="hover:text-lightOrange">Kontakt</RouterLink>
                <RouterLink :to="{ path: '/'}" class="hover:text-lightOrange">Blog</RouterLink>
                <RouterLink :to="{ path: '/login'}" class="hover:text-lightOrange">Zaloguj/Zarejestruj</RouterLink>
            </div>
        </div> -->
  </nav>
  <hr class="hidden md:block mx-6x" />
</template>

<script>
import { RouterLink } from "vue-router";
import hamburger from "../stores/hamburger.js";
export default {
  mounted() {
    hamburger();
  },
  components: { RouterLink },
};
</script>

<style></style>
