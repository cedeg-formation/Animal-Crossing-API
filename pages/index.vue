<template>
  <div class="p-6">
    <h2 class="text-emerald-400 text-2xl">Liste des habitants</h2>
    <Animal
      :villagers="{
        0: { name: 'Nom', item: 'Jojo' },
        1: { name: 'Personalité', item: 'Sympa' },
        2: { name: 'Anniversaire', item: '03/02/1960' },
        3: { name: 'id', item: '01' },
      }"
      :url="'https://acnhapi.com/v1/images/villagers/1'"
    />
  </div>
</template>
<script setup lang="ts"></script>
