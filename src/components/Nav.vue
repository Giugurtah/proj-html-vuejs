<template>
  <div id="nav" class="container d-flex justify-content-between align-content-center py-2">
      <div id="logo" class="fw-bold">
        <div class="d-inline-block text-end rounded-half brand_color_light brand_color_lighter_txt pe-1 py-2">N E X</div>
        <div class="d-inline-block ps-1">G E N</div>
      </div>
      <div class="my-2">
        <ul>
          <li v-for="(data, index) in navData" :key="index" class="uppercase aux_color_light_txt mx-3"> {{data}} </li>
        </ul>
        <div class="d-inline-block aux_color_lighter_txt uppercase brand_color py-1 px-3 rounded-2">Get in touch</div>
      </div>
  </div>
</template>

<script>
import navData  from "../assets/data/nav.js";
export default {
  name: 'Nav',
  data() {
    return {
      navData,
    }
  }
}
</script>

<style lang="scss">
#logo {
  div {
    width: 60px;
  }
}
</style>