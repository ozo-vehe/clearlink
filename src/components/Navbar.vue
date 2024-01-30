<script setup>
import logo from '../assets/img_01.png';

const links = [
  {
    name: 'products',
    url: '#',
  },
  {
    name: 'solutions',
    url: '#',
  },
  {
    name: 'resources',
    url: '#',
  },
  {
    name: 'pricing',
    url: '#',
  }
]
</script>

<template>
  <nav class="pt-10 px-24">
    <div
      class="nav_container flex flex-wrap gap-4 items-center justify-between bg-[#F2F4F7] py-3 px-8 rounded-[100px] border border-[#D0D5DD]">
      <div class="logo flex gap-[10px] items-center">
        <img :src="logo" alt="Logo">
        <p class="text-[24px] text-[#101828] flex font-[600]">ClearLink <span class="text-[#528BFF]">.</span></p>
      </div>

      <ul class="nav_links flex item-center gap-10">
        <li class="capitalize text-[#667085]" v-for="(link, index) in links" :key="index">
          <a :href="link.url" class="flex gap-[6px] items-center">
            {{ link.name }}
            <img class="w-4 h-4" src="https://img.icons8.com/ios-glyphs/667085/60/chevron-down.png" alt="chevron-down" />
          </a>
        </li>
      </ul>

      <div class="nav_btns flex gap-2 items-center">
        <button
          class="flex py-[12px] px-6 rounded-[100px] bg-white border border-[#98a2b3] text-[#101828] font-[600] shadow-[0px_1px_2px_0px_rgba(16,24,40,0.05)]">Talk
          to sales</button>
        <button
          class="flex py-[12px] px-6 rounded-[100px] bg-[#175CD3] border border-[#98a2b3] text-white font-[600] shadow-[0px_1px_2px_0px_rgba(16,24,40,0.05)]">Sign
          up for free</button>
      </div>

      <div class="mobile_nav relative hidden">
        <img class="w-8 h-8" src="https://img.icons8.com/ios-filled/100/menu--v6.png" alt="menu--v6" />

        <div class="mobile_menu absolute -right-8 h-[0px] overflow-hidden p-0 top-12 w-[340px] bg-white rounded-[8px] border-[#D0D5DD]">
          <ul class="nav_links w-full">
            <li class="capitalize text-[#667085] my-4 bg-gray-100 py-2 px-4 rounded-[3px]" v-for="(link, index) in links" :key="index">
              <a :href="link.url" class="flex gap-[6px] items-center justify-between">
                {{ link.name }}
                <img class="w-4 h-4" src="https://img.icons8.com/ios-glyphs/667085/60/chevron-down.png"
                  alt="chevron-down" />
              </a>
            </li>
          </ul>
          <div class="nav_btns px-4 flex flex-wrap gap-2 items-center justify-center w-full">
            <button
              class="w-full flex justify-center py-[14px] px-6 rounded-[100px] bg-white border border-[#98a2b3] text-[#101828] font-[600] shadow-[0px_1px_2px_0px_rgba(16,24,40,0.05)]">Talk
              to sales</button>
            <button
              class="w-full justify-centerflex py-[14px] px-6 rounded-[100px] bg-[#175CD3] border border-[#98a2b3] text-white font-[600] shadow-[0px_1px_2px_0px_rgba(16,24,40,0.05)]">Sign
              up for free</button>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped></style>
