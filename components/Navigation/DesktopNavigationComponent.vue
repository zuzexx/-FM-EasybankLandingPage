<template>
  <section class="z-20 w-full h-20 absolute top-0 left-0 mx-auto bg-white">
    <div
      class="w-10/12 max-w-6xl mx-auto h-full flex justify-between items-center"
    >
      <img alt="easybank logo" src="@/assets/images/logo.svg" class="h-5" />
      <ul class="flex justify-center items-center space-x-14">
        <li
          v-for="text in texts"
          :key="text"
          class="capitalize hover:border-b-4 text-neutral-grayish-blue hover:border-b-primary-bright-cyan text-lg hover:text-primary-dark-blue py-6 hover:cursor-pointer"
        >
          {{ text }}
        </li>
      </ul>
      <Button text="Request Invite"></Button>
    </div>
  </section>
</template>
<script setup lang="ts">
const texts = ['home', 'about', 'contact', 'blog', 'careers'];
</script>
