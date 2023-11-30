<script setup lang="ts">
import { appName } from '~/constants'

useHead({
  title: appName,
})
</script>

<template>
  <VitePwaManifest />
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<style>
html, body , #__nuxt{
  height: 100vh;
  margin: 0;
  padding: 0;
}

html.dark {
  background: #222;
  color: white;
}

h1{
  font-size: 20px;
  font-weight: bold;
  margin: 20px 0;
}
p{
  font-size: 16px;
  line-height: 1.5;
  margin: 10px 0;
}
</style>
