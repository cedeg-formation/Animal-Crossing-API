<template>
  <Animal :villager="dataVillager" :url="dataVillager['image_uri']" />
</template>

<script setup>
const route = useRoute();
const id = route.params.id;

const dataVillager = await $fetch("https://acnhapi.com/v1/villagers/" + id);
</script>
