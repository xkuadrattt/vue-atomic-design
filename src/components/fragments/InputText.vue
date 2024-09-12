<template>
  <input
    :type="type"
    class="input-text"
    :placeholder="placeholder"
    :data-variant="variant"
    :required="required"
  />
</template>

<script setup lang="ts">
import { InputText } from "@/model/type";

const props = withDefaults(defineProps<InputText>(), {
  type: "text",
  placeholder: "text is not blank",
  variant: "primary",
  required: true,
});
</script>
