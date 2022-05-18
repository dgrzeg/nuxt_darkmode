<template>
  <div :class="{ 'dark-mode': isDarkMode }">
    <Nav />
    <Heading />
    <Cards />
  </div>
</template>

<script setup lang="ts">
const { isDarkMode } = useDarkMode()
</script>

<style>
* {
  margin: 0;
  padding: 0;
  font-family: Georgia;
}
.dark-mode {
  background-color: black !important;
  color: white !important;
}
.dark-mode-nav {
  background-color: rgb(73, 72, 72) !important;
  color: white !important;
}
</style>
