<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <div id="body" class="">
    <aside id="nav" class="w-64" aria-label="Sidebar">
      <div
        class="overflow-y-auto py-4 px-3 bg-gray-100 rounded dark:bg-gray-700"
      >
        <ul class="space-y-2">
          <li>
            <router-link tag="li" to="/files">Files</router-link>
          </li>
          <li>
            <router-link tag="li" to="/files">Files</router-link>
          </li>
        </ul>
      </div>
    </aside>
    <router-view />
  </div>
</template>

<style lang="postcss">
#nav li {
  @apply flex items-center p-2 text-base font-normal text-gray-900 rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-500;
}
</style>
