<template>
  <div class="shadow card">
    <div
      class="absolute px-4 py-1 shadow-md left-8 top-8 rounded-4rem bg-white flex gap-2 text-black font-black">
      {{
          rating
      }} <div class="i-carbon-star-filled text-primary"></div>
    </div>
    <img class="w-full"
      :src="img"
      :alt="heading">
    <h3 class="text-black text-lg capitalize text-center">
      {{ heading }}
    </h3>
    <button class="rounded-50% bg-primary p-2">
      <div class="i-akar-icons-cart text-white" />
    </button>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  heading: string,
  img: string,
  rating: number
}>()
</script>

<style scoped>
.card {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: .5rem;
  padding: 1rem;
  border-radius: .25rem;
}

.card:hover {
  transition: box-shadow .3s;
  box-shadow: 10px 10px 32px rgba(0, 0, 0, 0.25);
}
</style>