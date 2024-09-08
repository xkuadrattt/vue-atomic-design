<template>
  <p :class="[leading, className]">{{ title }}</p>
</template>

<script setup lang="ts">
import { ParagraphUi } from "@/model/type";

const props = withDefaults(defineProps<ParagraphUi>(), {
  title: "Paragraph Ui",
});
</script>
