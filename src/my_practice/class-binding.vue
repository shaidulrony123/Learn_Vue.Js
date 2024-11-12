<script setup>
  const bgIndigo = 'bg-indigo-400';
  const bgYellow = 'bg-yellow-400';
  const bgGreen = 'bg-green-400';

  const weekday = false

  const colors ={
    bgColor : 'bg-teal-100',
    borderColor : 'border-teal-500',
    textColor : 'text-teal-900',

  }

const messegeType = 'success';
if('error' === messegeType){
  colors.bgColor = 'bg-red-100';
  colors.borderColor = 'border-red-500';
  colors.textColor = 'text-red-900';
}else if('success' === messegeType){
  colors.bgColor = 'bg-green-100';
  colors.borderColor = 'border-green-500';
  colors.textColor = 'text-green-900';
}else if('warning' === messegeType){
  colors.bgColor = 'bg-yellow-100';
  colors.borderColor = 'border-yellow-500';
  colors.textColor = 'text-yellow-900';
}
</script>

<template>
 <section class="container mx-auto flex items-center flex-col">
   <h1 class="text-center text-2xl py-10">Class and Style Buinding</h1>

   <section class="flex space-x-10">
    <div class="w-1/3 p-28 h-16" :class="bgIndigo"></div>
    <div class="w-1/3 p-28 h-16" :class="bgYellow"></div>
    <div class="w-1/3 p-28 h-16" :class="bgGreen"></div>
   </section>

   <section class="mt-10">
    <div class="h-16 w-96 flex items-center justify-center text-white" :class="[weekday ? 'bg-red-600' : 'bg-green-600', weekday ? 'text-4xl' : 'text-3xl' , weekday ? 'font-bold' : 'font-semibold']">
      It's a Week day
    </div>
   </section>

   <section class="mt-10">
    <div class=" border-t-4 rounded-b px-4 py-3 shadow-md" :class="[colors.bgColor, colors.borderColor, colors.textColor]">
      <p>This is a success alert</p>
      <p>Make sure to read the <a class="underline" href="https://tailwindcss.com/docs/customizing-colors">documentation</a></p>
    </div>
   </section>


 </section>
</template>

<style scoped>

</style>

