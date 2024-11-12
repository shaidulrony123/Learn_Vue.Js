<script setup>
  const bgOrange = ' background-color:rgba(255, 165, 0, 0.5)';
  const bgGreen = 'background-color: rgba(0, 128, 0, 0.5)';
  const bgBlue = 'background-color: rgba(0, 0, 255, 0.5)';
  const bgIndigo = 'background-color: rgba(75, 0, 130, 0.5)';
  const bgRed = 'background-color: rgba(255, 0, 0, 0.5)';

const colors ={
  borderColor: 'rgba(0, 0, 0, 0.5)',
  color: 'rgba(1, 654, 0, 0.5)',
  backgroundColor: 'rgba(0, 0, 324, 0.5)',
}
const weekday = true
</script>

<template>
 <section class="container mx-auto flex items-center flex-col">
  <h1 class="text-center text-2xl py-10">style binding</h1>
    <section class="flex space-x-10">
      <div class="w-1/3 h-16 w-96" :style="bgOrange"></div>
      <div class="w-1/3 h-16 w-96" :style="bgGreen"></div>
      <div class="w-1/3 h-16 w-96" :style="bgBlue"></div>
    </section>

    <section class="mt-10">
    <div class="h-16 w-96 flex items-center justify-center text-white" :style = "weekday==true ?[bgIndigo, 'font-size: 20px']:bgRed">
      It's a Week day
    </div>
   </section>

 </section>
</template>

<style scoped>

</style>

