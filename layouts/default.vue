<template>
  <div>
    <Navbar></Navbar>
    <div class="bg-base-200">
      <slot></slot>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
export default {
  setup() {
    useHead({
      title: "Nuxt",
    });
  },
};
</script>
