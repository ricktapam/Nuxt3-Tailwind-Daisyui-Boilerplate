<template>


    <Navbar></Navbar>
    <NuxtPage />
    <Footer></Footer>

</template>

<script setup lang="ts">
useHead({
    title: 'Nuxt',
    meta: [
        { name: 'description', content: 'A boilerplate Nuxt-project' }
    ],
})
</script>

<style>
.page-enter-active,
.page-leave-active {
    transition: all 0.2s;
}

.page-enter-from,
.page-leave-to {
    opacity: 0;
    filter: blur(1rem);
}
</style>