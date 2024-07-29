<template>
  <div class="forpc">
    <div class="fixed bottom-0 h-[90px] w-full bg-white flex items-center justify-center gap-[10px] z-30">
      <div class="pt-[10px]">
        <a href="/home">
          <img src="@/assets/images/top/common/wine.webp" alt="" class="h-[100px]">
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