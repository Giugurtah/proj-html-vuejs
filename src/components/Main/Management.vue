<template>
    <section id="menagement" class=" p-standard text-center">
        <h6 class="uppercase brand_color_txt fw-bold ">how it works in pratice</h6>
        <h1><div class="d-inline-block brand_color_base brand_color_txt px-2">Process</div> Management</h1>
        <p class="d-inline-block w-50 color_gray_txt mt-4">We work with innovative methodologies to ensure that the entire reformatting process is done from start to finish as planned.</p>
        <div class="px-5 mt-5 position-relative">
            <div class="break_line position-absolute top-0 start-50 translate-middle"></div>
            <ManagementCard v-for="(item, index) in menagementData" :key="index" :item="item" :itemIndex="index"/>
        </div>
    </section>
</template>

<script>
import menagementData from "../../assets/data/menagement.js";
import ManagementCard from "./ManagmentCard.vue";
export default {
  name: 'Management',
  components: {
      ManagementCard,
  },
  data() {
      return {
        menagementData
      }
  }
}
</script>

<style lang="scss">
@import "../../assets/style/_variables.scss";
.break_line {
    height: 3px;
    width: 100%;
    background-color:  $brand_color_lighter;
}
</style>