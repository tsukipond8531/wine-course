<template>
  <div class="w-[235px] min-w-[235px] shadow-lg overflow-hidden bg-white">
    <div>
      <img :src="imageSrc" loading="lazy" alt="">
    </div>
    <div class="h-[27px] w-[150%] -translate-x-7 -translate-y-[20px] -rotate-6 bg-white"></div>
    <div class="p-[10px] pt-0">
      <p class="text-[10px]">{{ date }}</p>
      <p class="text-[13px] pt-[8px] line-clamp-1">{{ title }}</p>
      <p class="text-[11px] pt-[21px] line-clamp-2">{{ excerpt }}</p>
      <button class="text-[14px] p-[10px] w-full border border-black mt-[21px] relative">
        この記事を見る
        <span class="absolute top-1/2 left-[calc(100%-20px)] transform -translate-y-1/2">&#8640;</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imageSrc: {
      type: String,
      required: true
    },
    date: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    excerpt: {
      type: String,
      required: true
    }
  }
}
</script>