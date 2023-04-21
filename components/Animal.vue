<template>
  <ul class="flex flex-col flex-wrap justify-center">
    <List
      class="flex justify-center flex-wrap"
      v-for="(info, key) in villager"
      :title="key"
      :item="info"
    />
    <li class="flex justify-center p-6">
      <NuxtLink :to="'/villager/' + villager['id']">
        <img alt="image d'un personnage" :src="url"
      /></NuxtLink>
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
