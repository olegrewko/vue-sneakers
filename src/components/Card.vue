<script setup>
import { ref } from 'vue';

defineProps({
  title: String,
  img: String,
  price: Number,
//   isAdded: Boolean
});

const isLiked = ref(false);
const isAdded = ref(false);

// const onClick = () => {
//   isLiked.value = !isLiked.value;
  
// };
// const onClick = () => {
  
//   isAdded.value = !isAdded.value;
// };
</script>

<template>
  <div
    class="relative flex flex-col w-full border border-slate-100 rounded-sm p-10 cursor-pointer transition hover:shadow-sm hover:transform hover:-translate-y-1"
  >
    <div @click="onClick" class="absolute top-8 left-8">
      <img :src="!isLiked ? '/like-1.svg' : '/like-2.svg'" alt="Favorite" />
    </div>
    <img :src="img" class="w-full" alt="Sneaker" />
    <p>{{ title }}</p>
    <div class="flex justify-between mt-5">
      <!-- <div class=" flex space-x-0 gap-1"> -->
        <span class="text-slate-300">Цена:</span>
        <span class="text-sm">{{ price }} руб.</span>
      <!-- </div> -->
      <img :src="!isAdded ? 'plus.svg' : 'checked.svg'" alt="Plus" />
    </div>
  </div>
</template>
