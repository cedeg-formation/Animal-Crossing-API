<template>
  <ul>
    <List
      v-for="villager in villagers"
      :title="villager['name']"
      :item="villager['item']"
    />
    <li>
      <img alt="image d'un personnage" :src="url" />
    </li>
  </ul>
</template>

<script>
export default {
  name: "Animal",
  props: {
    villagers: [],
    url: String,
  },
};
</script>

<style scoped></style>
