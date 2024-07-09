<template>
  <main class="relative">
    <Nav />
    <section class="xl:padding-l wide:padding-r padding-b">
      <Hero />
    </section>
    <section class="padding">
      <PopularProducts />
    </section>
    <section class="padding">
      <SuperQuality />
    </section>
    <section class="padding-x py-10">
      <Services />
    </section>
    <section class="padding">
      <SpecialOffer />
    </section>
    <section class="bg-pale-blue padding">
      <CustomerReviews />
    </section>
    <section class="padding-x sm:py-32 py-16 w-full">
      <Subscribe />
    </section>
    <section class="bg-black padding-x padding-t pb-8">
      <TheFooter />
    </section>
  </main>
</template>


<script setup lang="ts">
import Nav from '@/components/Nav.vue'
import Hero from '@/sections/Hero.vue';
import PopularProducts from '@/sections/PopularProducts.vue'
import SuperQuality from '@/sections/SuperQuality.vue'
import Services from '@/sections/Services.vue'
import SpecialOffer from '@/sections/SpecialOffer.vue'
import CustomerReviews from '@/sections/CustomerReviews.vue'
import Subscribe from '@/sections/Subscribe.vue'
import TheFooter from '@/sections/TheFooter.vue'

</script>