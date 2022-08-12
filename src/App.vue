<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import SideBarVue from "./components/SideBar.vue";
</script>

<template>
  <div id="body" class="flex">
    <div id="nav" class="inline-flex lg:flex-col flex-row w-screen lg:h-screen lg:w-auto content-center bg-gray-200">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="postcss" scoped>
a {
  @apply font-normal hover:font-bold rounded-lg p-1;
}

a.router-link-exact-active {
  @apply bg-yellow-200;
}
</style>
