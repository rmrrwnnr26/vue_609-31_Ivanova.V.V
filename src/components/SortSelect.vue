<script setup>
defineProps({
  modelValue: { type: String, required: true },
  options: { type: Array, required: true },
});

defineEmits(["update:modelValue"]);
</script>

<template>
  <select
    :value="modelValue"
    @change="$emit('update:modelValue', $event.target.value)"
    class="flex items-center border pl-3 gap-2 bg-white border-gray-500/30 h-[52px] rounded-md outline-none"
  >
    <option
      v-for="option in options"
      :key="option.value"
      :value="option.value"
    >
      {{ option.label }}
    </option>
  </select>
</template>