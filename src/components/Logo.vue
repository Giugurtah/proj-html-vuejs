<template>
    <div class="logo fw-bold">
      <div class="d-inline-block text-end rounded-half brand_color_light_txt brand_color_base pe-1 py-2">N E X</div>
      <div :class="colorText" class="d-inline-block ps-1">G E N</div>
    </div>
</template>

<script>
export default {
  name: 'Logo',
  props: ['colorText'],
}
</script>

<style lang="scss">
.logo {
  div {
    width: 60px;
  }
}
</style>