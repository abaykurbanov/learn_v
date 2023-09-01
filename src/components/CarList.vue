<script setup>
import CarItem from '@/components/CarItem.vue'

const carsArray=[
  {
    brand:"bmw",
    price:"2000000",
    year:1994,
    color: "#FF0000",
    image: "https://scaleartsin.com/cdn/shop/products/1994-BMW-Alpina-E34-B10-BiTurbo-red-1-43-Solido-diecast-scale-model-miniature-automobile-3_grande.jpg?v=1665650499"
  },
]
</script>

<template>
<section class="cars" v-for="car in carsArray" :key="car">
  <CarItem :car="car"/>
</section>
</template>

<style scoped></style>