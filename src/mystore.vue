<script setup>
  // const message = 'WelCome To Vue 3.0.0-beta.1';
  // const date = 'Thu sep 1 2024';


  // function getDate() {
  //   const date = new Date();
  //   return date.toDateString();
  // }
// import
import {data} from './data/data.js';

const image =[
  {
    imagee: 'https://www.pexels.com/photo/autumn-leaves-and-chestnuts-arrangement-28949941/',
    title: 'shaiduls portfolio',
    link: 'https://www.pexels.com/photo/autumn-leaves-and-chestnuts-arrangement-28949941/'
    // link: 
  },
  {
    imagee: 'https://www.pexels.com/photo/autumn-leaves-and-chestnuts-arrangement-28949941/',
    title: 'shaiduls portfolio 1',
    link: 'https://www.pexels.com/'
  },
  {
    imagee: 'https://www.pexels.com/photo/autumn-leaves-and-chestnuts-arrangement-28949941/',
    title: 'shaiduls portfolio 2',
    link: 'https://www.pexels.com/'
  }

]
</script>

<template>
  <!-- output -->
<!-- <section>
  <div class="container mx-auto flex items-center min-h-screen flex-col">
  <h1 class="text-4xl">{{ data.message }}</h1>
  <h2 class="mt-10 text-xl font-bold">Today date is <span>{{ data.date }} </span></h2>
  <h2 class="mt-10 text-xl font-bold">Today task is <span>{{ data.tasks.length }} </span></h2>

</div>
</section> -->

<!-- images section -->
 <section>
  <div class="container">
    <h1 class="text-4xl font-bold flex mb-10">Image Container</h1>

<section class="flex">
  <div class="grid grid-cols-3 gap-4 ">
      <div class="w-96">
        <img :title="image[0].title" src="./assets/pexels-mikhail-nilov-6943095.jpg" alt="image">
        <h1 class="text-4xl text-left mt-5 font-bold">{{ image[0].title }}</h1>
        <a target="_blank" :href="image[0].link">
          <p class="btn btn-primary bg-red-600 w-32 rounded mt-5 p-2 text-white">Image Source</p>
        </a>
      </div>
    </div>
  <div class="grid grid-cols-3 gap-4">
      <div class="w-96">
        <img :title="image[1].title" src="./assets/pexels-minan1398-1313814.jpg" alt="image">
        <h1 class="text-4xl text-left mt-5 font-bold">{{ image[1].title }}</h1>
        <a target="_blank" :href="image[1].link">
          <p class="btn btn-primary bg-red-600 w-32 rounded mt-5 p-2 text-white">Image Source</p>
        </a>
      </div>
    </div>
  <div class="grid grid-cols-3 gap-4">
      <div class="w-96">
        <img :title="image[2].title" src="./assets/pexels-samaraagenstvo-feeria-1261201-2399097.jpg" alt="image">
        <h1 class="text-4xl text-left mt-5 font-bold">{{ image[2].title }}</h1>
        <a target="_blank" :href="image[2].link">
          <p class="btn btn-primary bg-red-600 w-32 rounded mt-5 p-2 text-white">Image Source</p>
        </a>
      </div>
    </div>
</section>


  </div>
 </section>
<!-- images section -->
</template>

<style scoped>
/* style css */
</style>
