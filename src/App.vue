<script setup>
  // 1
  const persons=[
    {
      id: 1,
      name: 'Shaidul Islam',
      profilePhoto: 'https://www.pexels.com/photo/autumn-leaves-and-chestnuts-arrangement-28949941/',
      jobTile: 'Full Stack Developer'
    },
    {
      id: 2,
      name: 'Shaidul Islam',
      profilePhoto: 'https://www.pexels.com/photo/autumn-leaves-and-chestnuts-arrangement-28949941/',
      jobTile: 'Full Stack Developer'
    },
    {
      id: 3,
      name: 'Shaidul Islam',
      profilePhoto: 'https://www.pexels.com/photo/autumn-leaves-and-chestnuts-arrangement-28949941/',
      jobTile: 'Full Stack Developer'
    }
  ] 
 
</script>

<template>
 <section class="container mx-auto">
  <!-- 1 -->
 <div class="mb-16 text-center">
  <h2 class="mb-4 text-center text-2xl font-bold">Team Members</h2>
  <p class="text-gray-500 w-8/12 mx-auto">Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, laudantium.</p>
 </div>
 <div class="grid gap-12 items-center grid-cols-3">
  <div class="space-y-4 text-center">
    <img class="w-64 mx-auto h-64 object-cover rounded-xl w-64 h-64" src="./assets/pexels-mikhail-nilov-6943095.jpg" alt="">
    <div>
      <h4>Shaidul Islam</h4>
      <span class="block text-sm text-gray-400">Full Stack Developer</span>
    </div>
  </div>
  <div class="space-y-4 text-center">
    <img class="w-64 mx-auto h-64 object-cover rounded-xl w-64 h-80" src="./assets/pexels-mikhail-nilov-6943095.jpg" alt="">
    <div>
      <h4>Shaidul Islam</h4>
      <span class="block text-sm text-gray-400">Full Stack Developer</span>
    </div>
  </div>
  <div class="space-y-4 text-center">
    <img class="w-64 mx-auto h-64 object-cover rounded-xl w-64 h-64" src="./assets/pexels-mikhail-nilov-6943095.jpg" alt="">
    <div>
      <h4>Shaidul Islam</h4>
      <span class="block text-sm text-gray-400">Full Stack Developer</span>
    </div>
  </div>
 </div>
 </section>
</template>

<style scoped>

</style>

