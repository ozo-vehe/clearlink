<script setup>
import shopify from '../assets/img_11.png';
import coinbase from '../assets/img_06.png';
import dropbox from '../assets/img_07.png';
import intercom from '../assets/img_08.png';
import marvel from '../assets/img_09.png';
import automatic from '../assets/img_10.png';
import recorder from '../assets/img_12.png';
import noise from '../assets/img_13.png';
import calendar from '../assets/img_14.png';
import lock from '../assets/img_15.png';
import community from '../assets/img_16.png';
import arrow from '../assets/img_17.png';

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
  <section class="about_clearlink py-24 px-16 flex flex-wrap gap-4 justify-center">
    <div class="header_container w-[700px]">
      <header class="mb-20">
        <p class="text-[#175cd3] text-[16px] font-[600]">The ClearLink Advantage</p>
        <h2 class="text-[40px] font-[600]">Why choose ClearLink?</h2>
        <p class="text-[17px] font-[400] text-[#667085]">In a world where connection is everything, ClearLink takes the
          lead. Our cutting-edge video conferencing app offers:</p>
      </header>

      <div class="services_container">
        <div class="services flex flex-wrap gap-12">
          <div class="service flex flex-col gap-4 items-start w-[280px]">
            <img class="border border-[#eaecf0] rounded-full w-10 h-10 p-2 bg-[#F9FAFB]" :src="recorder" alt="Recorder">
            <div class="service_text">
              <h3 class="mb-1 text-[16px] font-[600] text=[#101828]">Crystal-clear HD video</h3>
              <p class="font-[400] text-[14px] text-[#475467]">No more pixelation or blurriness – just stunning, lifelike
                clarity that brings your team closer in meetings.</p>
            </div>
          </div>

          <div class="service flex flex-col gap-4 items-start w-[280px]">
            <img class="border border-[#eaecf0] rounded-full w-10 h-10 p-2 bg-[#F9FAFB]" :src="noise" alt="Noise">
            <div class="service_text">
              <h3 class="mb-1 text-[16px] font-[600] text=[#101828]">Noise-canceling audio</h3>
              <p class="font-[400] text-[14px] text-[#475467]">Say goodbye to distractions with our advanced audio tech for crisp, interruption-free conversations.</p>
            </div>
          </div>

          <div class="service flex flex-col gap-4 items-start w-[280px]">
            <img class="border border-[#eaecf0] rounded-full w-10 h-10 p-2 bg-[#F9FAFB]" :src="calendar" alt="Calendar">
            <div class="service_text">
              <h3 class="mb-1 text-[16px] font-[600] text=[#101828]">Scheduling made easy</h3>
              <p class="font-[400] text-[14px] text-[#475467]">Streamline your agenda with ClearLink's intuitive scheduling. Set up meetings, send invitations, and receive reminders in one place.</p>
            </div>
          </div>

          <div class="service flex flex-col gap-4 items-start w-[280px]">
            <img class="border border-[#eaecf0] rounded-full w-10 h-10 p-2 bg-[#F9FAFB]" :src="lock" alt="Lock">
            <div class="service_text">
              <h3 class="mb-1 text-[16px] font-[600] text=[#101828]">Bank-grade security</h3>
              <p class="font-[400] text-[14px] text-[#475467]">Your privacy is our priority with bank-grade security protocols safeguarding your meetings and data from unwanted intruders.</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="service_images w-[400px]">
      <img class="w-[250px]" :src="arrow" alt="Arrow image">
      <img :src="community" alt="Community">
    </div>
  </section>
</template>

<style scoped>
</style>
