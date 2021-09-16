<template>
  <div class="management_card d-inline-block position-relative align-top">
    <div class="d-inline-block position-absolute top-0 start-50 translate-middle rounded-style brand_color_lighter brand_color_txt fw-bold">{{ String(this.itemIndex+1).padStart(2, '0') }}</div>
    <h4 class="fw-bold mb-3 mt-5 mx-3"> {{item.title}} </h4>
    <p class="color_gray_txt"> {{item.text}} </p>
  </div>
</template>

<script>
export default {
  name: 'ManagementCard',
  props: ['item', 'itemIndex'],
}
</script>

<style lang="scss">
.management_card {
    width: 20%;
}
</style>