<template>
  <header class="padding-x py-8 absolute z-10 w-full">
    <nav class="flex justify-between items-center max-container">
      <a href="/">
        <img :src="headerLogo" alt="Logo" :width="130" :height="29" />
      </a>
      <ul class="flex-1 flex justify-center items-center gap-16 max-lg:hidden">
        <li v-for="item in navLinks" :key="item.label">
          <a :href="item.label" class="font-montserrat leading-normal text-lg text-slate-gray">
            {{ item.label }}
          </a>
        </li>
      </ul>
      <div class="hidden max-lg:block">
        <img :src="hamburger" alt="Hamburger" :width="25" :height="25"

        />
      </div>
    </nav>
  </header>
</template>

<script setup lang="ts">
import { headerLogo } from '@/assets/images';
import { hamburger } from '@/assets/icons';
import { navLinks } from '@/constants';


</script>