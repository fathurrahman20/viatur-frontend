<script setup>

import {ref} from "vue";
import ItemsCard from "./../ItemCard.vue";

const items = ref([
  {id: 1, title: "Atomic Habits", img: "item-1.jpg", category: "Motivation & Self-Help"},
  {id: 2, title: "The Psychology of Money", img: "item-2.jpg", category: "Motivation & Self-Help"},
  {id: 3, title: "Finding The Next Starbucks", img: "item-3.jpg", category: "Business & Technology"},
])
</script>

<template>
  <div class="container px-4 mx-auto my-16 md:px-12">
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">New Items</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
      <ItemsCard v-for="item in items" :key="item.id" :title="item.title" :category="item.category" :image="item.img" />


<!--      <div class="w-full px-1 my-1 md:w-1/2 lg:my-4 lg:px-4 lg:w-1/3">-->
<!--        <div class="overflow-hidden border border-gray-200 rounded-xl">-->
<!--          <a href="details.html">-->
<!--            <div class="m-4 overflow-hidden rounded-xl">-->
<!--              <img alt="Placeholder" class="block w-full h-auto" src="@/assets/img/item-1.jpg" />-->
<!--            </div>-->
<!--          </a>-->

<!--          <header class="px-4 mb-4 leading-tight">-->
<!--            <h1 class="text-lg">-->
<!--              <a class="font-semibold text-black no-underline hover:underline" href="/public/details.html"> Atomic Habits </a>-->
<!--            </h1>-->
<!--            <span class="block text-sm font-light text-gray-500 no-underline"> Motivation & Self-Help </span>-->
<!--          </header>-->
<!--        </div>-->
<!--      </div>-->
<!--      <div class="w-full px-1 my-1 md:w-1/2 lg:my-4 lg:px-4 lg:w-1/3">-->
<!--        <div class="overflow-hidden border border-gray-200 rounded-xl">-->
<!--          <a href="details.html">-->
<!--            <div class="m-4 overflow-hidden rounded-xl">-->
<!--              <img alt="Placeholder" class="block w-full h-auto" src="@/assets/img/item-2.jpg" />-->
<!--            </div>-->
<!--          </a>-->

<!--          <header class="px-4 mb-4 leading-tight">-->
<!--            <h1 class="text-lg">-->
<!--              <a class="font-semibold text-black no-underline hover:underline" href="#"> The Psychology of Money </a>-->
<!--            </h1>-->
<!--            <span class="block text-sm font-light text-gray-500 no-underline"> Motivation & Self-Help </span>-->
<!--          </header>-->
<!--        </div>-->
<!--      </div>-->
<!--      <div class="w-full px-1 my-1 md:w-1/2 lg:my-4 lg:px-4 lg:w-1/3">-->
<!--        <div class="overflow-hidden border border-gray-200 rounded-xl">-->
<!--          <a href="details.html">-->
<!--            <div class="m-4 overflow-hidden rounded-xl">-->
<!--              <img alt="Placeholder" class="block w-full h-auto" src="@/assets/img/item-3.jpg" />-->
<!--            </div>-->
<!--          </a>-->

<!--          <header class="px-4 mb-4 leading-tight">-->
<!--            <h1 class="text-lg">-->
<!--              <a class="font-semibold text-black no-underline hover:underline" href="#"> Finding The Next Starbucks </a>-->
<!--            </h1>-->
<!--            <span class="block text-sm font-light text-gray-500 no-underline"> Computers & Technology </span>-->
<!--          </header>-->
<!--        </div>-->
<!--      </div>-->
    </div>
  </div>
</template>