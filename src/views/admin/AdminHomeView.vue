<script setup>
import { ref } from 'vue';


const showSidebar = ref(true);


const toggleShowSidebar = () => {

  showSidebar.value = !showSidebar.value;

}



</script>


<template>

  <div class="grid grid-cols-12 grid-rows-12 h-screen">
    <!-- Header -->
    <header class="col-start-3 col-span-10 p-2 flex items-center">

      <nav class="flex justify-between items-center px-10 w-full">

        <div class="text-2xl cursor-pointer" @click="toggleShowSidebar">
          <span class="pi pi-align-justify"></span>
        </div>
        <ul class="flex gap-x-10 text-4xl items-center">
          <li class="relative cursor-pointer"><span class="pi pi-comment"></span>
            <span
              class="text-sm bg-green-500 px-2.5 text-white font-semibold py-1 rounded-full absolute -top-2 -right-2">7</span>
          </li>
          <li class="relative cursor-pointer"><span class="pi pi-bell"></span>
            <span
              class="text-sm bg-red-500 px-2.5 text-white font-semibold py-1 rounded-full absolute -top-2 -right-2">1</span>
          </li>
          <li class="cursor-pointer"><span class="pi pi-user"></span></li>
        </ul>
      </nav>
    </header>

    <!-- sidebar -->

    <div class="row-start-1 row-span-12 col-start-1 col-span-2 bg-red-500 p-2">
      <aside>sidebar</aside>
    </div>

    <!-- main content -->
    <div class="row-span-10 col-span-10 bg-green-500 p-2">
      content
    </div>
    <!-- footer -->
    <footer class="row-start-12 row-span-1  col-start-3 col-span-10 bg-yellow-700 p-2">
      footer
    </footer>
  </div>


</template>