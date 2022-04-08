<template>
  <div class="container">
    <aside class="w-1/12 h-full bg-black">
      <h1>test</h1>
    </aside>
    <section class="w-11/12 h-full bg-red-600">
      <h1>section 2</h1>
    </section>
  </div>
</template>

<script>
export default {
  async asyncData ({ $http }) {
    const test = await $http.$get('/api/test')
    return {
      test
    }
  }
}
</script>

<style scoped>
.container{
  @apply w-full h-full border-4 flex;
}
</style>
