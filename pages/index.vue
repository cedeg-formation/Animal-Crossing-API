<template>
  <div class="p-6">
    <h2 class="text-emerald-400 text-2xl">Liste des habitants</h2>
    <Animal
      v-for="dataVillage in dataVillagers"
      :villager="dataVillage"
      :url="dataVillage['image_uri']"
    />
    <!--    <Animal
      :villagers="{
        0: { title: 'Nom', item: 'Jojo' },
        1: { title: 'Personalité', item: 'Sympa' },
        2: { title: 'Anniversaire', item: '03/02/1960' },
        3: { title: 'id', item: '01' },
      }"
      :url="'https://acnhapi.com/v1/images/villagers/1'"
    />-->
  </div>
</template>
<script setup>
const dataVillagers = await $fetch("https://acnhapi.com/v1/villagers");
</script>
