<script setup>
import LinkCard from './LinkCard.vue';


</script>

<template>
   <div class="bg-gray-100 mt-30">
      <div class="m-5 mb-0 bg-indigo-950 p-10 rounded-lg flex flex-col gap-5 -translate-y-10 md:flex-row md:mx-auto lg:max-w-150 ">
         <input type="text" class="w-full h-14 bg-white rounded-lg text-amber-500 px-3 font-medium"
            placeholder="Shorten a link here">
         <button class="w-full h-14 bg-cyan-400 rounded-lg text-white md:w-65">Shorten It!</button>
      </div>
      <div class="m-5 mb-0 flex flex-col gap-5 -translate-y-10 md:mx-auto lg:max-w-150">
         <LinkCard originalLink="https://frontendmentor.io" shortedLink="https://rel.ink/k4lKyk" isOdd="true" />
         <LinkCard originalLink="https://frontendmentor.io" shortedLink="https://rel.ink/k4lKyk" />
         <LinkCard originalLink="https://frontendmentor.io" shortedLink="https://rel.ink/k4lKyk" isOdd="true" />
      </div>
   </div>

</template>

<style scope></style>