<template>
  <section id="services" class="aux_color_lighter p-standard">
    <div class="container">
        <h6 class="uppercase brand_color_txt fw-bold">our buiseness areas</h6>
        <h1>Exellence in <div class="d-inline-block brand_color_base brand_color_txt px-2">Services</div></h1>
        <div class="d-flex justify-content-between align-items-center color_gray_txt my-4">
            <p class="w-75">
                We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.
            </p>
            <div class="button_style">see all</div>
        </div>
        <div class="row g-4">
            <ServicesCard v-for="(item, index) in servicesData" :key="index" :item="item"/>
        </div>
    </div>
  </section>
</template>

<script>
import ServicesCard from "./ServicesCard.vue";
import servicesData from "../../assets/data/services.js";
export default {
  name: 'Services',
  components: {
      ServicesCard,
  },
  data() {
      return {
          servicesData,
      }
  }
}
</script>

<style>
</style>