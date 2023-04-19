<template>
  <div class="p-6">
    <h2 class="text-emerald-400 text-2xl">Liste des habitants</h2>
    <ul>
      <List :title="'Nom'" :item="'Jojo'" />
      <List :title="'Personalité'" :item="'Sympa'" />
      <List :title="'Anniversaire'" :item="'03/02/1960'" />
      <List :title="'id'" :item="'01'" />
      <li>
        <img
          alt="image d'un personnage"
          src="https://acnhapi.com/v1/images/villagers/1"
        />
      </li>
    </ul>
  </div>
</template>
<script setup lang="ts"></script>
