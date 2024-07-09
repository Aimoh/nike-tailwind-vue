<template>
  <section class="max-container flex justify-center flex-wrap gap-9 w-full">
    <div v-for="service in services" :key="service.label" class="flex flex-1 sm:w-[350px] sm:min-w-[350px] w-full">
      <ServiceCard :imgURL="service.imgURL" :label="service.label" :subtext="service.subtext" />
    </div>
  </section>
</template>

<script setup lang="ts">
import { services } from '@/constants'
import ServiceCard from '@/components/ServiceCard.vue'
</script>
