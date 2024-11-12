<script setup>
  const location = 'Dhaka';
  const weather = 's';
</script>

<template>
 <!-- <section class="container mx-auto flex items-center flex-col">
    <h1 class="text-center text-2xl py-10">Logic in Vue</h1>
  <div class="w-1/3  p-10 flex items-center flex-col space-y-10">
    <h1 class="text-3xl">{{ location }}</h1>
    <h2 class="text-2xl" v-if="weather=='s'">Weather: Sunny</h2>
    <h2 class="text-2xl" v-else-if="weather=='pc'">Weather: Partly Cloudy</h2>
    <h2 class="text-2xl" v-else-if="weather=='r'">Weather: Rainy</h2>
    <h2 class="text-2xl" v-else-if="weather=='t'">Weather: Thunderstorm</h2>
    <h2 class="text-2xl" v-else>Weather: Clear</h2>
    <img title="Thunderstorm" v-if="weather =='t'" src="./assets/pexels-mikhail-nilov-6943095.jpg" alt="!">
    <img title="Sunny" v-if="weather =='s'" src="./assets/pexels-samaraagenstvo-feeria-1261201-2399097.jpg" alt="!">
    <img title="Partly Cloudy" v-if="weather=='pc'" src="./assets/pexels-minan1398-1313814.jpg" alt="!">
  </div>
 </section> -->

 <!-- group condition -->

 <section class="container mx-auto flex items-center flex-col">
    <h1 class="text-center text-2xl py-10">Logic in Vue</h1>
  <div class="w-1/3  p-10 flex items-center flex-col space-y-10">
    <h1 class="text-3xl">{{ location }}</h1>

   <template v-if="weather=='s'">
        <h2 class="text-2xl">Weather: Sunny</h2>
        <img title="sunny" src="./assets/pexels-mikhail-nilov-6943095.jpg" alt="!">
   </template>

    <template v-else-if="weather=='pc'">
        <h2 class="text-2xl" >Weather: Partly Cloudy</h2>
        <img title="Partly Cloudy" src="./assets/pexels-minan1398-1313814.jpg" alt="!">
    </template>

    <template v-else-if="weather=='t'">
        <h2 class="text-2xl">Weather: Thunderstorm</h2>
        <img title="Thunderstorm" src="./assets/pexels-samaraagenstvo-feeria-1261201-2399097.jpg" alt="!">
    </template>

  </div>
 </section>
</template>

<style scoped>
</style>

