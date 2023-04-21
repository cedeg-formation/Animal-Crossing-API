<template>
  <ul>
    <List v-for="(info, index) in villager" :title="index" :item="info" />
    <li>
      <img alt="image d'un personnage" :src="url" />
    </li>
  </ul>
</template>

<script>
export default {
  name: "Animal",

  props: {
    villager: [Object],
    url: String,
  },
  methods: {},
};
</script>
