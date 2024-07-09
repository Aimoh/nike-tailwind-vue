<template>
  <button
    :class="buttonClasses">
    {{ label }}
    <img v-if="iconURL" :src="iconURL" alt="arrow right icon" class="ml-2 rounded-full bg-white w-5 h-5" />
  </button>
</template>

<script setup lang="ts">
import { computed } from 'vue';

const props = defineProps({
  label: String,
  iconURL: String,
  backgroundColor: String,
  textColor: String,
  borderColor: String,
  fullWidth: Boolean,
})

const buttonClasses = computed(() => {
  const baseClasses = 'flex justify-center items-center gap-2 px-7 py-4 border font-montserrat text-lg leading-none rounded-full';
  const bgClass = props.backgroundColor ? props.backgroundColor : 'bg-coral-red';
  const textClass = props.textColor ? props.textColor : 'text-white';
  const borderClass = props.borderColor ? props.borderColor : 'border-coral-red';
  const fullWidthClass = props.fullWidth ? 'w-full' : '';

  return `${baseClasses} ${bgClass} ${textClass} ${borderClass} ${fullWidthClass}`;
})
</script>
