<script setup>
import { ref, computed } from 'vue'
const props = defineProps({
    num: Number

})

</script>

<template>
    <div class = "Title">
        <h1>
            <slot name = "text">default title text</slot>
        </h1>
    </div>
</template>

<style scoped>
.Title h1{
    margin-top: 2%;
    text-align: center;
    color: #530ff0;
    text-decoration: solid;
    font-size: 60px;
    font-family: 'Courier New', Courier, monospace;
    
}

</style>