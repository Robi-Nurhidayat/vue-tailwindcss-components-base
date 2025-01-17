<script setup>


</script>


<template>

    <div class="grid grid-cols-12 grid-rows-12 h-screen">
        <!-- Header -->
        <header class="col-start-3 col-span-10 bg-blue-500 p-2">

            <nav>header</nav>
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