<template>
  <!-- section che contine le notizie sul cliente -->
  <section id="news" class="container p-standard">
    <!-- Titolo + intestazione -->
    <h6 class="intestazione_style brand_color_txt">our editorial content</h6>
    <h1 class="title_style">Latest <div class="underline_title brand_color_base brand_color_txt">News</div></h1>
    <!-- Contenuto sottotitolo + bottone -->
    <div class="d-flex justify-content-between align-items-center color_gray_txt my-4">
        <p class="w-75 m-0">
           Every week we publish content about what is best in the business world.
        </p>
        <button class="button_style">see all</button>
    </div>
    <!-- Stampa card -->
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