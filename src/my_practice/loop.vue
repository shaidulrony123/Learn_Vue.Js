<script setup>
  // 1
  const items= [1,2,3,4,5]  

  // 2
  const tasks = [
    "Task 1",
    "Task 2",
    "Task 3",
    "Task 4",
    "Task 5"
  ]

// 3
const arrytasks=[
  {id:1, name:"Task 1", age:20, status:"pending"},
  {id:2, name:"Task 2", age:21, status:"success"},
  {id:3, name:"Task 3", age:22, status:"success"},
  {id:4, name:"Task 4", age:23, status:"pending"},
  {id:5, name:"Task 5", age:24, status:"pending"},
  {id:6, name:"Task 6", age:25, status:"pending"},
]
function getFilterTask(){
  return arrytasks.filter(arrytask=>"pending"===arrytask.status)
}
</script>

<template>
 <section class="container mx-auto">
  <!-- 1 -->
  <!-- <div v-for="item in items">{{ item }}</div> -->

  <!-- 2 -->
  <!-- <h1 class="text-center text-2xl" v-for="(task, index) in tasks">{{ index+1 }}. {{ task }}</h1> -->
  <!-- 3 -->
   <h3 class="text-center text-2xl" v-for="arrytask in getFilterTask()" :key="arrytask.id">{{ arrytask.id }} {{ arrytask.status }}</h3>
   <h1></h1>
 </section>
</template>

<style scoped>

</style>

