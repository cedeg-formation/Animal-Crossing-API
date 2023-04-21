<template>
  <li>
    <p>
      <span class="font-bold text">{{ title }} :</span> {{ item }}
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
