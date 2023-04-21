<template>
  <li>
    <p v-if="title === 'name'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item["name-EUfr"] }}
    </p>
    <p v-else>
      <span class="font-bold text">{{ title }} :</span>
      {{ item }}
    </p>
  </li>
</template>

<script>
export default {
  name: "List",
  props: {
    title: String,
    item: String,
  },
};
</script>
