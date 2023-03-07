<template>

    
    <h1>{{naam}}</h1> 
    <h1>{{ counts }}</h1>
    <button @click="incF">Increase</button>

</template>

<script setup>
import { inject } from "vue";


let naam = inject('names', )
// let counts = inject("count")
let incF = inject("incF")

</script>