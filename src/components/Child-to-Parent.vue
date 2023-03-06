<template>
    <!-- // Child Component -->
    <div class="bg-stone-600 w-3/4 rounded-xl h-56 flex flex-col justify-center items-center m-5 shadow-2xl">
    <h1 class="p-2 sm:w-1/4 md:w-2/3 text-[#00FF00] ">Child</h1>
        <!-- <div  class="w-3/4 bg-gray-600 border-red-500 border-4 rounded-lg text-red-500 flex justify-center items-center font-extrabold text-2xl h-24">{{ count }}</div> -->
        <button class="p-2 m-2 border-4 border-[#00FF00]" @click="$emit('increaseCount')">Increase Parent Count</button>
    </div>   


</template>



<script setup>


</script>