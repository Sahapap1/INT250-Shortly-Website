<script setup>
import { ref } from "vue";

const show = ref(false);

const toggle = () => {
  show.value = !show.value;
};
</script>

<template>
  <!-- Nav Container -->
  <nav>
    <!-- Flex Container for all items -->
    <div>
      <!-- Flex Container for Logo/Menu -->
      <div class="flex justify-between items-center p-5 md:px-10 lg:px-0 lg:justify-around">
        <div class="flex items-center gap-15">
          <!-- Logo -->
          <img src="../assets/logo.svg" alt="" />
          <!-- Left Menu -->
          <div class="hidden lg:flex gap-5 font-bold">
            <a href="">Features</a>
            <a href="">Pricing</a>
            <a href="">Resources</a>
          </div>
        </div>

        <!-- Right Button Menu -->

        <i @click="toggle" class="fa-solid text-gray-500 lg:hidden!" :class="show ? 'fa-x order-3' : 'fa-bars'"></i>
        <div class=" lg:flex gap-5 font-bold items-center" :class="show ? 'flex ml-auto mr-3' : 'hidden'">
          <a href="">Login</a>
          <a href="" class="text-white rounded-4xl bg-cyan-400 px-5 py-2">Sign up</a>
        </div>


        <!-- @todo Hamburger Button -->
      </div>
    </div>
  </nav>
</template>

<style scope></style>
