<template>
  <section id="nav" class="container d-flex justify-content-between align-content-center py-2">
      <Logo :colorText="''" />
      <div class="my-2">
        <ul>
          <li v-for="(data, index) in navData" :key="index" class="uppercase color_gray_txt mx-3"> {{data}} </li>
        </ul>
        <div class="button_style">Get in touch</div>
      </div>
  </section>
</template>

<script>
import Logo from "../Logo.vue";
import navData  from "../../assets/data/nav.js";
export default {
  name: 'Nav',
  components: {
    Logo,
  },
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