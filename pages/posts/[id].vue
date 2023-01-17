<template>
  <div class="container mx-auto text-center py-8">
    <h1 class="text-5xl mb-8 max-w-[70%] mx-auto font-bold">{{ post.title }}</h1>
    <div class="flex justify-center items-center mb-8">
      <div class="avatar">
        <div class="w-16 rounded-full ring ring-primary ring-offset-base-100 ring-offset-2">
          <img src="https://placeimg.com/192/192/people" />
        </div>
      </div>
      <div class="ml-4 text-left">
        <p class="font-bold text-xl">John Doe</p>
        <p class="text-md">2023-01-1</p>
      </div>
    </div>
    <p class="text-xl max-w-[60%] mx-auto">{{ post.body }}</p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = "https://jsonplaceholder.typicode.com/posts/" + id;
const { data: post } = await useFetch(uri);
</script>
