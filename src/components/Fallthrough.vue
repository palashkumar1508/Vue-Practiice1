<template>
    <div>
        Without custom attrs
    </div>
    <div v-bind="$attrs" class="shadow-xl shadow-amber-300 rounded-lg ">
        Custom $Attrs
    </div>


</template>
<script>
export default{
    inheritAttrs:false
}

</script>
<script setup>


</script>