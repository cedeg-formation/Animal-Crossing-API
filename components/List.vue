<template>
  <li>
    <p>
      <span class="font-bold">{{ title }} :</span> {{ item }}
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
