<template>
  <!-- Template card utilizzata in News.vue -->
  <div class="news_card col-4">
     <!--Bckground + contenuto (ricevuti tramite props)  -->
    <div class="position-relative" 
      v-bind:style="{'background-image': 'url(' + require('../../assets/img/' + this.item.img) + ')'}">
      <p class="position-absolute bottom-0 mx-5 mb-5 text-center color_white_txt fw-bolder fs-3 lh-sm">{{item.text}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NewsCard',
  props: ['item'],
}
</script>

<style lang="scss">
.news_card {
  // Styling custom della simgola card
  div {
    height: 400px;
    background-position: center;
    background-size: cover;

    border-radius: 20px;
  }
  // Style di aggiunta overlay
  div:before {
    content: "";
    position: absolute;
    left: 0; right: 0;
    top: 0; bottom: 0;
    background: rgba(0,0,0,.5);
    border-radius: 20px;
  }
}
</style>