<template>
  <li>
    <p v-if="title === 'name'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item["name-EUfr"] }}
    </p>
    <p class="hidden" v-else-if="title === 'file-name'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item }}
    </p>
    <p class="hidden" v-else-if="title === 'icon_uri'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item }}
    </p>
    <p class="hidden" v-else-if="title === 'image_uri'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item }}
    </p>
    <p class="hidden" v-else-if="title === 'bubble-color'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item }}
    </p>
    <p class="hidden" v-else-if="title === 'text-color'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item }}
    </p>
    <p v-else-if="title === 'catch-translations'">
      <span class="font-bold text">{{ title }} :</span>
      {{ item["catch-EUfr"] }}
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
    item: [String, Object, Array, Number],
  },
};
</script>
