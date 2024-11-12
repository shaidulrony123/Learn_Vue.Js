<script setup>
    const number= 55;
    const animal = 'baby';
    // const searchUrl = 'https://www.pexels.com/search/';

    // const searchUrl = 'https://www.pexels.com/search/'+ animal;
    
    const searchUrl = 'https://www.pexels.com/search/';
</script>

<template>
 <section>
    <!-- number divided by 10 -->
    <h1 class="text-4xl text-center font-bold">{{ number }} /10 = {{ number/10 }}</h1>
    <!-- condition using ternary -->
     <h2 class="text-4xl text-center font-bold text-green-600 mt-5">{{ number}} is  {{ number %2 ==0 ?'Even': 'Odd' }}</h2>
 </section>
 <!-- search animal -->
  <section class="mt-5">
    <!-- <a target="_blank" :href="searchUrl+animal">
        search for {{ animal }}
    </a> -->
    <!-- <a target="_blank" :href="searchUrl">
        search for {{ animal }}
    </a> -->
    <a target="_blank" :href="`https://www.pexels.com/search/${animal}`">
        search for {{ animal }}
    </a>
  </section>
</template>

<style scoped>
</style>

