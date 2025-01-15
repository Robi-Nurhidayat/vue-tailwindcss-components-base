<script setup>

</script>

<template>

<section class="flex justify-center items-center h-screen bg-gray-100">
    <div class=" w-[500px] border bg-white px-5 pt-5 pb-6 rounded">
        <h1 class="mb-10 text-3xl font-semibold text-center text-gray-800">Login Dahulu</h1>
        <form action="" class="flex flex-col gap-y-2">

            <div class="flex flex-col gap-y-1">
                <label for="email " class="text-2xl text-gray-800">Email</label>
                <input type="text" class="outline-none border px-2 py-2 rounded text-lg text-gray-600">
            </div>
            <div class="flex flex-col gap-y-1">
                <label for="password " class="text-2xl text-gray-800">Password</label>
                <input type="text" class="outline-none border px-2 py-2 rounded text-lg text-gray-600">
            </div>
            <div class="pt-4">
                <button class="bg-blue-500 hover:bg-blue-600 w-full py-2 text-white text-2xl font-semibold rounded">Login</button>
            </div>
        </form>
    </div>
</section>

</template>