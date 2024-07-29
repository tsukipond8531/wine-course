<template>
  <div class="forpc">
    <div class="fixed bottom-0 h-[90px] w-full bg-white flex items-center justify-center gap-[10px] z-30">
      <div class="pt-[10px]">
        <a href="/home">
          <img src="@/assets/images/top/common/wine.webp" alt="" class="h-[100px]">
        </a>
      </div>
      <div class="pt-[10px]">
        <a href="/real">
          <img src="@/assets/images/top/common/real.webp" alt="" class="h-[100px]">
        </a>
      </div>
      <div>
        <img src="@/assets/images/top/common/contact.webp" alt="" class="h-[69px]">
      </div>
      <div @click="scrollToTop" class="absolute right-[10px] bottom-[5px] cursor-pointer">
        <img src="@/assets/images/top/common/top.webp" alt="Go to top" class="h-[50px]">
      </div>
    </div>
  </div>
  <div class="forsp">
    <div class="flex items-center h-[120rem] fixed bottom-0 z-30 bg-opacity-60 bg-white">
      <div class="w-1/2">
        <a href="/home">
          <img src="@/assets/images/top/common/wine_sp.webp" alt="" class="w-full">
        </a>
      </div>
      <div class="w-1/2">
        <a href="/real">
          <img src="@/assets/images/top/common/real_sp.webp" alt="" class="w-full">
        </a>
      </div>
      <div @click="scrollToTop" class="absolute right-[10px] bottom-[125rem] cursor-pointer">
        <img src="@/assets/images/top/common/top.webp" alt="Go to top" class="h-[70rem]">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }
  }
}
</script>