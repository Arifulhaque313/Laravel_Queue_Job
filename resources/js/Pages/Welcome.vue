<script setup>
import { Head, Link } from '@inertiajs/vue3';

const props = defineProps({
    data:{
        type:Object
    }
})

</script>

<template>
    <Head title="Welcome" />
    <div class="max-w-7xl mx-auto my-10 p-10 border border-violet-600 hover:border-yellow-600 rounded-md">
        <h1 class="text-center text-3xl font-bold">Laravel Queue Job</h1>
        
        <div class="flex justify-center items-center mt-20 gap-4">
            <p v-if="data.length>0" class="text-white rounded-full bg-red-600 h-8 w-8 text-center pt-1">{{ data.length }}</p>
            <a href="/test-mail" class="bg-green-600 hover:bg-green-700 px-6 py-1 hover:scale-125 rounded-md shadow-md text-white">Send Mail</a>
            <a href="/" class="bg-blue-600 hover:bg-blue-700 px-6 py-1 hover:scale-125 rounded-md shadow-md text-white">Home</a>
        </div>
    </div>

</template>
