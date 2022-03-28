<template>
  <div>
    <NuxtPage/>
  </div>
</template>

<style>
html, body {
  height: 100%;
}
#__nuxt, #__nuxt > div {
  height: 100%;
}
</style>

<script setup>
const route = useRoute()

useMeta({
  title: computed(() => `${route.meta.title}`)
})
</script>
