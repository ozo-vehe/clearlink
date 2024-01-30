<script setup>
import shopify from '../assets/img_11.png';
import coinbase from '../assets/img_06.png';
import dropbox from '../assets/img_07.png';
import intercom from '../assets/img_08.png';
import marvel from '../assets/img_09.png';
import automatic from '../assets/img_10.png';

const social_images = [
  {
    url: shopify,
    name: 'Shopify'
  },
  {
    url: coinbase,
    name: 'Coinbase'
  },
  {
    url: dropbox,
    name: 'Dropbox'
  },
  {
    url: intercom,
    name: 'Intercom'
  },
  {
    url: marvel,
    name: 'Marvel'
  },
  {
    url: automatic,
    name: 'Automatic'
  },
]
</script>

<template>
  <section class="social_proof items-center py-24 px-16">
    <h2 class="text-[#475467] text-[18px] text-center mb-12">Join 1,500+ companies already video conferencing the ClearLink way</h2>
    <div class="social_images flex flex-wrap gap-x-4 gap-y-8 justify-around items-center">
      <img v-for="(image, index) in social_images" :key="index" :src="image.url" :alt="image.name">
    </div>
  </section>
</template>

<style scoped>
</style>
