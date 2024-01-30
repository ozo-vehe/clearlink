<script setup>
import shopify from '../assets/img_11.png';
import star from '../assets/img_05.png';
import community from '../assets/img_18.png';
import user from '../assets/img_19.png';
import right from '../assets/img_20.png';
import left from '../assets/img_21.png';
</script>

<template>
  <section class="testimony bg-[#F9FAFB] py-24 px-16 flex flex-wrap gap-12 justify-center">
    <div class="header_container w-[600px]">
      <header class="mb-20">
        <img class="w-[100px] mb-5" :src="shopify" alt="Shopify">
        <div class="stars flex items-center gap-2">
          <img v-for="i in 5" :key="i" :src="star" alt="Star">
        </div>
      </header>

      <div class="testimonies">
        <div class="testimony w-full font-[500] leading-[43px] text-[32px] text-[#101828]">
          <p>ClearLink has upgraded our remote meetings. High-quality video, screen sharing, and top-notch security make it essential for our team.</p>

          <div class="user mt-12 w-full flex justify-between items-center">
            <div class="user_details flex items-end w-fit gap-3">
              <img class="w-10" :src="user" alt="User">
              <div class="user_name flex flex-col">
                <p class="text-[16px] leading-[20px] font-[600] text-[#101828]">Sarah Thompson</p>
                <p class="text-[14px] leading-[20px] font-[400] text-[#475467]">Project Manager, Shopify</p>
              </div>
            </div>

            <div class="arrow flex items-center gap-5">
              <img class="cursor-pointer w-[40px] border border-[#D1E9FF] backdrop-blur-[4px] bg-white/90 rounded-full p-2" :src="left" alt="Left arrow">
              <img class="cursor-pointer w-[40px] border border-[#D1E9FF] backdrop-blur-[4px] bg-white/90 rounded-full p-2" :src="right" alt="Right arrow">
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="service_images w-[450px]">
      <img :src="community" alt="Community">
    </div>
  </section>
</template>

<style scoped>
</style>
