<template>
  <div class="card">
    <AvatarUi />
    <div class="card-content">
      <h3 class="card-title">{{ title }}</h3>
      <p class="card-description">{{ desc }}</p>
    </div>
  </div>
</template>

<script setup lang="ts">
import { title } from "process";
import AvatarUi from "../fragments/AvatarUi.vue";
import { CardAvatar } from "@/model/type";

const props = withDefaults(defineProps<CardAvatar>(), {
  title: "User",
  desc: "Guest",
});
</script>
