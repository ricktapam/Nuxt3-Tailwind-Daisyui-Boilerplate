<template>
  <div class="container mx-auto py-8">
    <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-4 gap-0 md:gap-4">
      <div v-for="p in posts.slice(0, 12)" class="mx-auto">
        <PostCard :post="p"> </PostCard>
      </div>
    </div>
  </div>
</template>

<script setup>
const { data: posts } = await useFetch("https://jsonplaceholder.typicode.com/posts");
</script>
