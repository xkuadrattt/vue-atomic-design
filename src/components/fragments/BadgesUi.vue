<template>
  <div :class="[className, variant, 'badges']">
    <span>{{ title }}</span>
  </div>
</template>

<script setup lang="ts">
import { BadgesUi } from "@/model/type";

const props = withDefaults(defineProps<BadgesUi>(), {
  title: "Badges UI",
});
</script>
