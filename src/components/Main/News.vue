<template>
  <section id="news" class="container p-standard">
    <h6 class="uppercase brand_color_txt fw-bold mb-3">our editorial content</h6>
    <h1>Latest <div class="d-inline-block brand_color_base brand_color_txt px-2">News</div></h1>
    <div class="d-flex justify-content-between align-items-center color_gray_txt my-4">
        <p class="w-75 m-0">
           Every week we publish content about what is best in the business world.
        </p>
        <div class="button_style">see all</div>
    </div>
    <div class="row">
        <NewsCard v-for="(item, index) in newsData" :key="index" :item="item" />
    </div>
  </section>
</template>

<script>
import newsData from "../../assets/data/news.js";
import NewsCard from "./NewsCard.vue";
export default {
  name: 'News',
  components: {
      NewsCard
  },
  data() {
      return {
          newsData,
      }
  }
}
</script>

<style>

</style>