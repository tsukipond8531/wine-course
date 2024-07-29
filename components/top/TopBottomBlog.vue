<template>
  <section class="pt-[50px]">
    <h3 class="text-[#BB9966] border-b-2 border-b-[#BB9966] p-2 w-fit m-auto mb-[23px]">ワイン教室情報最前線</h3>
    <div class="bg-[url('/assets/images/top/bottom-blog/background.webp')] bg-no-repeat py-[100px]">
      <div class="max-w-[90%] lg:max-w-[1000px] m-auto flex justify-between overflow-auto gap-[20px]">
        <BlogCard :imageSrc="imageSrc1" date="2020.08.31" title="代官山スタジオ近辺のオススメスポット情報" :excerpt="excerpt1" />
        <BlogCard :imageSrc="imageSrc2" date="2020.08.31" title="代官山スタジオ近辺のオススメスポット情報" :excerpt="excerpt2" />
        <BlogCard :imageSrc="imageSrc3" date="2020.08.31" title="代官山スタジオ近辺のオススメスポット情報" :excerpt="excerpt3" />
        <BlogCard :imageSrc="imageSrc4" date="2020.08.31" title="代官山スタジオ近辺のオススメスポット情報" :excerpt="excerpt4" />
      </div>
      <button class="w-[250px] lg:w-[340px] bg-black text-white text-[12px] lg:text-[18px] p-[13px] block m-auto mt-[40px] relative">全ての記事を見る
        <span class="absolute top-1/2 left-[calc(100%-30px)] transform -translate-y-1/2 rotate-90">&#10095;</span>
      </button>
    </div>
  </section>
</template>

<script>
import BlogCard from '@/components/top/topBottomBlog/TopBlogCard2.vue'
import photo1 from '@/assets/images/top/bottom-blog/photo1.webp'
import photo2 from '@/assets/images/top/bottom-blog/photo2.webp'
import photo3 from '@/assets/images/top/bottom-blog/photo3.webp'
import photo4 from '@/assets/images/top/bottom-blog/photo4.webp'

export default {
  components: {
    BlogCard
  },
  data() {
    return {
      imageSrc1: photo1,
      imageSrc2: photo2,
      imageSrc3: photo3,
      imageSrc4: photo4,
      excerpt1: 'ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。',
      excerpt2: 'ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。',
      excerpt3: 'ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。',
      excerpt4: 'ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。ブログ記事抜粋。'
    }
  }
}
</script>
