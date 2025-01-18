<script setup>
import { ref } from 'vue';

import OrderIcon from '../../assets/order.svg';
import UserIcon from '../../assets/user.svg';
import StoreIcon from '../../assets/store.svg';

const showSidebar = ref(true);


const toggleShowSidebar = () => {

  showSidebar.value = !showSidebar.value;

}



</script>


<template>

  <div class="grid grid-cols-12 grid-rows-12 h-screen bg-[#f4f3fc]">
    <!-- Header -->
    <header class="col-start-3 col-span-10 p-2 flex items-center">

      <nav class="flex justify-between items-center px-10 w-full">

        <div class="text-2xl cursor-pointer" @click="toggleShowSidebar">
          <span class="pi pi-align-justify"></span>
        </div>
        <ul class="flex gap-x-5  items-center">
          <li
            class="flex justify-center items-center rounded relative cursor-pointer bg-[rgba(165,148,249,0.21)] w-[35px] h-[35px]">
            <span class="pi pi-comment text-lg text-[#210f7e]"></span>
            <span
              class="text-sm bg-[#A594F9] w-[25px] h-[25px] text-white font-semibold flex justify-center items-center rounded-full absolute -top-3 -right-3">7</span>
          </li>
          <li
            class="flex justify-center items-center rounded relative cursor-pointer bg-[rgba(165,148,249,0.21)] w-[35px] h-[35px]">
            <span class="pi pi-bell text-lg text-[#210f7e]"></span>
            <span
              class="text-sm bg-[#A594F9] w-[25px] h-[25px] text-white font-semibold flex justify-center items-center rounded-full absolute -top-3 -right-3">3</span>
          </li>
          <li class="cursor-pointer">
            Hello, Robi Nurhidayat
          </li>
        </ul>
      </nav>
    </header>

    <!-- sidebar -->

    <div class="row-start-1 row-span-12 col-start-1 col-span-2 flex bg-white justify-center shadow-sm">
      <aside class=" w-[80%] h-full ">
        <div class=" relative w-[70px] rounded-full p-4 bg-[rgba(255,82,59,0.29)] mb-10 mt-2">
          <img :src="StoreIcon" alt="store-icon">
          <span class="absolute font-semibold text-[#748E63] left-1 -bottom-5">RobiStore</span>
        </div>

        <ul class="flex flex-col gap-5">
          <li class="flex justify-between items-center cursor-pointer">
            <span class="text-xl font-medium text-gray-700">Dashboard</span>
            <span class="pi pi-home text-xl text-purple-500"></span>
          </li>
          <li class="flex justify-between items-center cursor-pointer">
            <span class="text-xl font-medium text-gray-700">Product</span>
            <span class="pi pi-gift text-xl text-purple-500"></span>
          </li>
          <li class="flex justify-between items-center cursor-pointer">
            <span class="text-xl font-medium text-gray-700">Pelanggan</span>
            <span class="pi pi-user text-xl text-purple-500"></span>
          </li>
        </ul>
      </aside>
    </div>

    <!-- main content -->
    <div class="row-span-10 col-span-10  px-10 overflow-auto">
      
      <div class="mb-5">
        <h1 class="text-gray-800 font-semibold">Dashboard</h1>
      <h5 class="text-gray-600">Welcome to Dashboard Page Robi Nurhidayat !</h5>
      </div>


      <div class="flex gap-7 flex-wrap">


        <!-- orders -->
        <div class="w-[330px] h-[172px] bg-white rounded shadow flex justify-center items-center">
          <div class="flex items-center gap-x-5">
            <div class="w-[90px] bg-[rgba(253,87,87,0.25)] rounded-full">
              <img :src="OrderIcon" alt="icon-order-dashboard" class="">
            </div>
            <div>
              <h5 class="font-bold text-[40px] ">10</h5>
              <span>Total Orders</span>
            </div>
          </div>
        </div>

        <!-- user -->
        <div class="w-[330px] h-[172px] bg-white rounded shadow flex justify-center items-center">
          <div class="flex items-center gap-x-5">
            <div class="w-[90px] bg-[rgba(253,87,87,0.25)] rounded-full">
              <img :src="UserIcon" alt="icon-order-dashboard" class="">
            </div>
            <div>
              <h5 class="font-bold text-[40px] ">10</h5>
              <span>Total users</span>
            </div>
          </div>
        </div>

        

      </div>
    </div>
    <!-- footer -->
    <footer class="row-start-12 row-span-1  col-start-3 col-span-10 p-2 flex items-center justify-center">
      <p class="text-center py-4 px-7 rounded bg-[rgba(165,148,249,0.21)] text-[#8670f8] font-medium">Created By Robi Nurhidayat</p>
    </footer>
  </div>


</template>