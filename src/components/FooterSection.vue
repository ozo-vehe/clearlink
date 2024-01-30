<script setup>
import { ref } from 'vue';
import logo from '../assets/img_01.png';
import apple_store from '../assets/img_24.png';
import google_play from '../assets/img_25.png';
import linkedin from '../assets/img_26.png';
import twitter from '../assets/img_27.png';
import facebook from '../assets/img_28.png';
import instagram from '../assets/img_29.png';
import github from '../assets/img_30.png';
import youtube from '../assets/img_31.png';
const show_answer = ref(false);
</script>

<template>
  <footer class="footer relative pt-24 flex flex-wrap gap-20 justify-center items-start">
    <div class="footer_desc flex px-16 flex-wrap items-start justify-between w-full gap-20">
      <div class="footer_logo w-[370px]">
        <div class="logo flex items-center gap-2 mb-5">
          <img :src="logo" alt="Logo">
          <p class="text-[20px] text-[#101828] flex font-[600]">ClearLink <span class="text-[#528BFF]">.</span></p>
        </div>

        <p class="text-[16px] text-[#475467] font-[400] leading-[25px]">ClearLink is your gateway to effortless, high-quality video conferencing. Join us in shaping the future of communication!</p>
      </div>

      <div class="footer_content flex flex-wrap max-w-[750px] items-start justify-around">
        <div class="product w-[150px]">
          <h3 class="text-[#667085] text-[14px] font-[600] mb-4">Product</h3>
          <ul class="text-[16px] text-[#475467] font-[600] flex flex-col gap-4">
            <li>Overview</li>
            <li>Features</li>
            <li>Solutions</li>
            <li>Tutorials</li>
            <li>Pricing</li>
          </ul>
        </div>

        <div class="company w-[150px]">
          <h3 class="text-[#667085] text-[14px] font-[600] mb-4">Company</h3>
          <ul class="text-[16px] text-[#475467] font-[600] flex flex-col gap-4">
            <li>About us</li>
            <li>Careers</li>
            <li>Press</li>
            <li>News</li>
            <li>Contact</li>
          </ul>
        </div>

        <div class="resources w-[150px]">
          <h3 class="text-[#667085] text-[14px] font-[600] mb-4">Resources</h3>
          <ul class="text-[16px] text-[#475467] font-[600] flex flex-col gap-4">
            <li>Blog</li>
            <li>Events</li>
            <li>Help centre</li>
            <li>Tutorials</li>
            <li>Support</li>
          </ul>
        </div>

        <div class="legal w-[150px]">
          <h3 class="text-[#667085] text-[14px] font-[600] mb-4">Legal</h3>
          <ul class="text-[16px] text-[#475467] font-[600] flex flex-col gap-4">
            <li>Terms</li>
            <li>Privacy</li>
            <li>Cookies</li>
            <li>Licenses</li>
            <li>Contact</li>
          </ul>
        </div>

        <div class="get_app w-[150px]">
          <h3 class="text-[#004eeb] text-[14px] font-[600] mb-4">Get the app</h3>
          <div class="mobile_store">
            <img class="w-full mb-2" :src="apple_store" alt="Apple store">
            <img class="w-full" :src="google_play" alt="Google play">
          </div>
        </div>
      </div>
    </div>

    <div class="footer_socials px-16 bg-[#F9FAFB] flex flex-wrap w-full gap-6 items-center py-12 justify-between">
      <p class="text-[14px] text-[#667085] font-[400]">© 2023 ClearLink. All rights reserved.</p>
      <div class="socials flex items-center gap-4">
        <img :src="linkedin" alt="LinkedIn">
        <img :src="twitter" alt="Twitter">
        <img :src="facebook" alt="Facebook">
        <img :src="instagram" alt="Instagram">
        <img :src="github" alt="GitHub">
        <img :src="youtube" alt="YouTube">
      </div>
    </div>
  </footer>
</template>

<style scoped>
.socials img {
  width: 20px;
  height: 20px;
}
@media screen and (max-width: 800px) {
  footer {
    padding: 0px;
  }
  .footer_desc {
    padding: 0px 20px;
  }
  header {
    margin-bottom: 40px;
  }
  .testimony > p {
    font-size: 28px;
    line-height: 1.5;
  }
  .footer_content {
    justify-content: flex-start;
    gap: 50px 10px;
  }
  .footer_socials {
    padding-left: 20px;
    padding-right: 20px;
  }
}
</style>
