<template>
  <div class="card_style col-4">
      <div class="color_white rounded-3 p-5">
          <div class="position-relative">
              <i class="fas fa-arrow-right brand_color_txt position-absolute end-0"></i>
              <i :class="item.icon" class="fas mb-3 brand_color_txt"></i>
              <h4 class="fw-bold mb-3"> {{item.title}} </h4>
              <p class="aux_color_light_txt"> {{item.text}} </p>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: ['item'],
}
</script>

<style lang="scss">
.card_style {
    i {
        font-size: 50px;
    }
    .fa-arrow-right {
        font-size: 30px
    }
}
</style>