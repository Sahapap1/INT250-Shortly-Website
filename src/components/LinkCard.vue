<script setup>
defineProps([
    "originalLink",
    "shortedLink",
    "isOdd"
])

</script>

<template>
    <div class="flex flex-col items-center gap-1 font-bold py-6 bg-white rounded-lg md:flex-row md:justify-between md:px-5 md:gap-5">
        <p>{{ originalLink }}</p>
        <p class="text-cyan-400 md:ml-auto">{{ shortedLink }}</p>
        <Button class="mt-1 px-8 py-2 rounded-lg text-white font-medium" :class="isOdd ? 'bg-cyan-400' : 'bg-indigo-950'">Copy</Button>
    </div>

</template>

<style scope></style>