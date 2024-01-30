<script setup>
import { ref } from 'vue';
import check from '../assets/img_22.png';
import video from '../assets/img_23.png';

const show_answer = ref(false);
</script>

<template>
  <section class="subscription relative pt-12 pb-20 px-16 flex flex-wrap gap-20 justify-center items-start">
    <div class="sub_info w-[500px]">
      <h2 class="text-[38px] font-[600] leading-[50px]">
        Ready to clear the path to perfect communication?
      </h2>

      <ul class="my-8 ml-4 flex flex-col gap-2">
        <li class="flex items-center gap-[7px]">
          <img class="w-[22px] h-[22px]" :src="check" alt="Check">
          <p class="text-[16px] font-[400] text-[#475467]">30 days free trial</p>
        </li>
        <li class="flex items-center gap-[7px]">
          <img class="w-[22px] h-[22px]" :src="check" alt="Check">
          <p class="text-[16px] font-[400] text-[#475467]">Cancel at any time</p>
        </li>
        <li class="flex items-center gap-[7px]">
          <img class="w-[22px] h-[22px]" :src="check" alt="Check">
          <p class="text-[16px] font-[400] text-[#475467]">Access to all features</p>
        </li>
        <li class="flex items-center gap-[7px]">
          <img class="w-[22px] h-[22px]" :src="check" alt="Check">
          <p class="text-[16px] font-[400] text-[#475467]">Peronalized onboarding</p>
        </li>
      </ul>

      <div class="sub_btns text-[14px] flex gap-2 items-center justify-start">
        <button
          class="flex py-[12px] px-6 rounded-[100px] bg-white border border-[#98a2b3] text-[#101828] font-[600] shadow-[0px_1px_2px_0px_rgba(16,24,40,0.05)]">Talk
          to sales
        </button>
        <button
          class="flex py-[12px] px-6 rounded-[100px] bg-[#175CD3] border border-[#98a2b3] text-white font-[600] shadow-[0px_1px_2px_0px_rgba(16,24,40,0.05)]">Sign
          up for free
        </button>
      </div>
    </div>

    <div class="sub_img w-[650px] h-[430px]">
      <img class="absolute w-[750px] right-0 top-8" :src="video" alt="Sub image">
    </div>
  </section>
</template>

<style scoped>
@media screen and (max-width: 1300px) {
  .subscription {
    padding-left: 20px;
    padding-right: 20px;
  }
  .sub_info {
    width: 430px;
  }
  .sub_info h2 {
    font-size: 32px;
    line-height: normal;
  }
  .sub_img {
    width: 500px;
  }
  .sub_img img {
    width: 550px;
  }
}

@media screen and (max-width: 1090px) {
  .sub_info {
    width: 400px;
  }
  .sub_info h2 {
    font-size: 30px;
    line-height: normal;
  }
  .sub_img {
    position: relative;
    width: 450px;
    height: 300px;
  }
  .sub_img img {
    top: 0px;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}

</style>
