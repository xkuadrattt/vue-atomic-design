<template>
  <RouterLink :to="link" class="sidebarlink">{{ title }}</RouterLink>
</template>

<script setup lang="ts">
import { LinkUi } from "@/model/type";

const props = withDefaults(defineProps<LinkUi>(), {
  link: "#",
  title: "link 1",
});
</script>
