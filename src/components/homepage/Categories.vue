<script setup>

import CategoriesCard from "./../CategoriesCard.vue";
import {ref} from "vue";

const categories = ref([
  {id: 1, title: 'Motivation & Self-Help', total: 2, image: "/src/assets/img/categories-1.jpg" },
  {id: 2, title: 'Computer & Technology', total: 1, image: "/src/assets/img/categories-2.jpg" },
  {id: 3, title: 'Business & Investing', total: 0, image: "/src/assets/img/categories-3.jpg" },
  {id: 4, title: 'Reference & Dictionary', total: 0, image: "/src/assets/img/categories-4.jpg" },
])

</script>

<template>

  <div class="container px-4 mx-auto my-16 md:px-12" id="categories">
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">Top Categories</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
    <CategoriesCard
        v-for="category in categories"
        :key="category.id"
        :title="category.title"
        :total="category.total"
        :image="category.image"/>
    </div>
  </div>

</template>