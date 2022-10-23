<script setup>
import Logo from './sub_component/Logo.vue';
import Navlink from './sub_component/NavigationLinks.vue'
import UserInfoButton from './sub_component/UserInfoButton.vue'
</script>

<template>

  <nav class="bg-white border-gray-200 px-2 sm:px-4 py-2.5 rounded dark:bg-gray-800">
    <div class="container flex flex-wrap items-center justify-between mx-auto my-2">
      <Logo/>
      <UserInfoButton/>
      <Navlink/>
    </div>
  </nav>

</template>