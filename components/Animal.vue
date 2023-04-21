<template>
  <ul>
    <List v-for="(info, key) in villager" :title="key" :item="info" />
    <li>
      <img alt="image d'un personnage" :src="url" />
    </li>
  </ul>
</template>

<script>
export default {
  name: "Animal",

  props: {
    villager: Object,
    url: String,
  },
  methods: {},
};
</script>
