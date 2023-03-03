<template>
   <div class="bg-stone-600 shadow-2xl w-3/4 flex flex-col justify-center items-center rounded-2xl m-5 p-7 text-black ">
        <input class="rounded-lg p-2 sm:w-2/3 md:w-1/3 flex justify-center items-center " v-model.number.lazy="num" type="number">
        <div class="">
            <button class="m-3" @click="increase">+1</button>
            <button class="m-3" @click="num = num+2">+2</button>
            <button class="m-3" @click="num = num+5">+5</button>
            <button class="m-3" @click="num = num-1">-1</button>
            <button class="m-3" @click="num = num-2">-2</button>
            <button class="m-3" @click="num = num-5">-5</button>
        </div>
        <!-- <div>{{ num }}</div> -->

        <h4 class="text-[#00FF00]" v-if="num">Old value : "{{ oldNum }}" & New value"{{ newNum }}"</h4>

   </div>
</template>

<script setup>
    import {ref, reactive, watch}  from 'vue';

    let num = ref()
    let oldNum = ref()
    let newNum = ref()

    function increase (){
        num.value++;
    }

    watch(num, (newValue, oldvalue)=>{
        oldNum = oldvalue ;
        newNum = newValue ;

    })

</script>

<style scoped>

button{
    @apply bg-black text-[#00FF00] border-red-500 border-4 shadow-2xl hover:scale-125
}

</style>
