<template>
  <div class="avatar">
    <img :src="src" alt="avatar" />
  </div>
</template>

<script setup lang="ts">
import { AvatarUi } from "@/model/type";

const props = withDefaults(defineProps<AvatarUi>(), {
  src: "@/assets/img/user-circle.svg",
});
</script>
