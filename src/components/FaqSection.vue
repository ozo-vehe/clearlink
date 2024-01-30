<script setup>
import { ref } from 'vue';

const show_answer = ref(false);
</script>

<template>
  <section class="faq py-24 px-16 flex flex-wrap gap-20 justify-center">
    <div class="header_container w-[400px]">
      <p class="text-[#175cd3] text-[16px] font-[600]">Support</p>
      <h2 class="text-[40px] font-[600]">FAQs</h2>
      <p class="text-[17px] font-[400] text-[#667085]">
        Everything you need to know about the product and billing. Can’t find the answer you’re looking for? <span
          class="underline underline-offset-4">Please chat to our friendly team.</span>
      </p>
    </div>

    <div class="questions w-[650px] flex flex-col">
      <div class="question_container flex items-start justify-between p-6 rounded-[16px] bg-[#f9fafb] border border-[#eaecf0] w-full">
        <div class="ma-w-[520px]">
          <h3 class="question text-[16px] text-[#101b2b] leading-[30px] font-[600]">How many participants can join a ClearLink video conference?</h3>
          <p class="answer text-[14px] text-[#475467] font-[400] leading-[23px]">
            ClearLink offers flexible meeting options. Depending on your subscription plan, you can host
            meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations
            and large-scale webinars, ensuring you have the right fit for your needs.
          </p>
        </div>

        <div @click="show_answer = !show_answer" class="cursor-pointer min-w-[24px] rounded-full h-[24px] icons flex border border-[#98A2B3] text-[#98A2B3] items-center justify-center">
          <span v-if="show_answer">-</span>
          <span v-else>+</span>
        </div>
      </div>

      <div class="group question_container flex items-start justify-between p-6 bg-white border-b border-[#eaecf0] w-full">
        <div class="max-w-[520px]">
          <h3 class="question text-[16px] text-[#101b2b] leading-[30px] font-[600]">Can I use ClearLink on multiple devices?</h3>
        </div>

        <div @click="show_answer = !show_answer" class="cursor-pointer min-w-[24px] rounded-full h-[24px] icons flex border border-[#98A2B3] text-[#98A2B3] items-center justify-center">
          <span>+</span>
        </div>
      </div>

      <div class="group question_container flex items-start justify-between p-6 bg-white border-b border-[#eaecf0] w-full">
        <div class="max-w-[520px]">
          <h3 class="question text-[16px] text-[#101b2b] leading-[30px] font-[600]">Is ClearLink compatible with other video conferencing platforms?</h3>
        </div>

        <div @click="show_answer = !show_answer" class="cursor-pointer min-w-[24px] rounded-full h-[24px] icons flex border border-[#98A2B3] text-[#98A2B3] items-center justify-center">
          <span>+</span>
        </div>
      </div>

      <div class="group question_container flex items-start justify-between p-6 bg-white border-b border-[#eaecf0] w-full">
        <div class="max-w-[520px]">
          <h3 class="question text-[16px] text-[#101b2b] leading-[30px] font-[600]">How does ClearLink ensure the security of my video conferences?</h3>
        </div>

        <div @click="show_answer = !show_answer" class="cursor-pointer min-w-[24px] rounded-full h-[24px] icons flex border border-[#98A2B3] text-[#98A2B3] items-center justify-center">
          <span>+</span>
        </div>
      </div>

      <div class="group question_container flex items-start justify-between p-6 bg-white border-b border-[#eaecf0] w-full">
        <div class="max-w-[520px]">
          <h3 class="question text-[16px] text-[#101b2b] leading-[30px] font-[600]">Do I need to download any software to use ClearLink?</h3>
        </div>

        <div @click="show_answer = !show_answer" class="cursor-pointer min-w-[24px] rounded-full h-[24px] icons flex border border-[#98A2B3] text-[#98A2B3] items-center justify-center">
          <span>+</span>
        </div>
      </div>

      <div class="group question_container flex items-start justify-between p-6 bg-white border-b border-[#eaecf0] w-full">
        <div class="max-w-[520px]">
          <h3 class="question text-[16px] text-[#101b2b] leading-[30px] font-[600]">What kind of customer support does ClearLink provide?</h3>
        </div>

        <div @click="show_answer = !show_answer" class="cursor-pointer min-w-[24px] rounded-full h-[24px] icons flex border border-[#98A2B3] text-[#98A2B3] items-center justify-center">
          <span>+</span>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
@media screen and (max-width: 800px) {
  .faq {
    padding: 40px 20px;
  }
}
</style>
