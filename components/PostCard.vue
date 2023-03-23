<template>
  <div class="card w-[22rem] bg-base-100 shadow-xl h-full">
    <figure><img src="https://picsum.photos/400/200" alt="" /></figure>
    <div class="card-body">
      <h2 class="card-title">{{ post.title }}</h2>
      <p>{{ post.body }}</p>
      <div class="card-actions justify-end">
        <NuxtLink :to="`/posts/${post.id}`" class="btn btn-primary"> Read More </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
const { post } = defineProps(["post"]);
</script>
