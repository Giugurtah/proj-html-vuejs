<template>
    <!-- Templkate singola card utilizzata in Team.vue -->
    <div class="col-6 mb-4">
        <img class="align-top rounded-2" :src="getImg()" alt="">
        <div class="d-inline-block ms-5">
            <!-- Nome + posizione (ricevute tramte props) -->
            <h2 class="color_white_txt lh-sm">{{item.name}}</h2>
            <h6 class="uppercase aux_color_light_txt">{{item.position}}</h6>
            <!-- Icone social -->
            <i class="fab fa-facebook-f me-2 rounded-style brand_color_txt aux_color_dark"></i>
            <i class="fab fa-twitter me-2 rounded-style brand_color_txt aux_color_dark"></i>
            <i class="fab fa-linkedin-in me-2 rounded-style brand_color_txt aux_color_dark"></i>
        </div>
    </div>
</template>

<script>
export default {
  name: 'TeamCard',
  props: ['item'],
  methods: {
      getImg() {
          return require("../../assets/img/" + this.item.img)
      }
  }
}
</script>

<style>
img {
    height: 100px;
}
</style>