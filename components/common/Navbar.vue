<template>
  <div>
    <div class="header_center bg-white">
      <div class="container flex justify-between items-center py-4">
        <div class="header_center_left flex items-center">
          <a href="/" class="mr-4">
            <img src="~/assets/images/header/logo.webp" alt="Logo" class="w-[300rem] lg:w-[217px]"/>
          </a>
          <div>
            <p class="text-sm hidden lg:block">
              自宅オンラインでも、リアルスタジオでも、
              <br />
              深まる・広がるワインスクール
            </p>
            <p class="text-[8px] ss:text-[10px] block lg:hidden">
              自宅オンラインでも、
              <br />
              リアルスタジオでも。
            </p>
          </div>
        </div>
        <div class="header_center_right hidden lg:flex space-x-4">
          <div class="flex items-center pb-2">
            <img src="~/assets/images/header/phone.webp" alt="Phone" />
          </div>
          <a href="/home">
            <img src="~/assets/images/header/home wine course.webp" alt="Home Wine Course" />
          </a>
          <a href="/real">
            <img src="~/assets/images/header/real studio course.webp" alt="Real Studio Course" />
          </a>
        </div>
        <button @click="toggleMenu" class="lg:hidden text-[60rem] focus:outline-none">
          &#9776;
        </button>
      </div>
    </div>
    <div v-if="isMenuOpen" class="fixed inset-0 z-40 bg-black bg-opacity-50" @click.self="toggleMenu">
      <div class="header_bottom_mobile fixed top-0 right-0 h-full w-[250px] bg-white shadow-lg z-50">
        <div class="container p-4 relative">
          <button @click="toggleMenu" class="absolute top-[10px] right-[10px] text-[60rem] z-20 focus:outline-none">
            &times;
          </button>
          <ul class="mt-12 space-y-4">
            <li><a href="/" class="block text-black">トップ</a></li>
            <li><a href="/real" class="block text-black">リアルスタジオコース</a></li>
            <li><a href="/home" class="block text-black">ホームワインコース</a></li>
            <li><a href="#" class="block text-black">初めての方へ</a></li>
            <li><a href="#" class="block text-black">料金</a></li>
            <li><a href="#" class="block text-black">アクセス</a></li>
            <li><a href="#" class="block text-black">ソムリエ（講師）</a></li>
            <li><a href="#" class="block text-black">Q&A</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="header_bottom hidden lg:block">
      <div class="container mx-auto">
        <ul class="flex space-x-4 list-none p-0 m-0">
          <li><a href="/" class="block text-black">トップ</a></li>
          <li><a href="/real" class="block text-black">リアルスタジオコース</a></li>
          <li><a href="/home" class="block text-black">ホームワインコース</a></li>
          <li><a href="#" class="block text-black">初めての方へ</a></li>
          <li><a href="#" class="block text-black">料金</a></li>
          <li><a href="#" class="block text-black">アクセス</a></li>
          <li><a href="#" class="block text-black">ソムリエ（講師）</a></li>
          <li><a href="#" class="block text-black">Q&A</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style scoped>
.header_center {
  background-color: #fff; /* Adjust as needed */
}

.header_bottom_mobile {
  position: fixed;
  top: 0;
  right: 0;
  height: 100%;
  width: 250px;
  background-color: #fff;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  z-index: 50; /* Ensure it is above other elements */
}

.header_bottom ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.header_bottom li,
.header_bottom_mobile li {
  padding: 10px;
}

.header_bottom li a,
.header_bottom_mobile li a {
  text-decoration: none;
  color: black;
  display: block; /* Ensure the clickable area is the entire list item */
}

.header_bottom_mobile .container {
  padding: 1rem;
}

.header_bottom_mobile button {
  position: absolute;
}
</style>
