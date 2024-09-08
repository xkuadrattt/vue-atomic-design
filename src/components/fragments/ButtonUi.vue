<template>
  <button :class="[className, variant, "btn"]">{{ title }}</button>
</template>

<script setup lang="ts">
import { ButtonUi } from "@/model/type";

const props = withDefaults(defineProps<ButtonUi>(), {
  title: "Read More",
});
</script>
