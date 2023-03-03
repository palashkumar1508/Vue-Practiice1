<template>
    <div class="w-3/4 rounded-2xl bg-stone-600 p-4 flex flex-col justify-center items-center">
        <h2 class="text-4xl p-4 text-[#00FF00]">Table</h2>
        <input type="number" class="rounded-xl md:w-1/3 sm:w-2/4 p-3" placeholder="Enter Number to get table" v-model.number.lazy="num" >
        <ul class="p-3 text-[#00FF00] border-2 border-[#00FF00] bg-black shadow-red-200 mt-4 text-xl rounded-2xl" v-show="num">
            <li v-for="i in 10 " :key="i">{{ num }} * {{ i }} = {{ num * i }}</li>

        </ul>
    </div>
    

</template>

<script setup>
import { ref } from "vue";
    let num = ref();


</script>