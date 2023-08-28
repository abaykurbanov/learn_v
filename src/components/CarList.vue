<script setup>
import CarItem from '@/components/CarItem.vue'
const carsArray=[
  {
    brand:"bmw",
    price:"2000000",
    year:1994,
    color: "#ff0000",
    image: "https://www.solido.com/wp-content/uploads/2020/12/s1803904-bmw-e36-coupe-m3-red-1994-01.jpg"
  },
]
</script>

<template>
<section class="cars" v-for="car in carsArray" :key="car">
<CarItem :car="car"/>
</section>
</template>

<style scoped></style>