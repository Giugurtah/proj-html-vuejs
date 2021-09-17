<template>
    <!-- Section contente le info sui servizi pfferti dal cliente -->
    <section id="services" class="aux_color_lighter p-standard">
        <div class="container">
            <!-- Titolo + intestazione -->
            <h5 class="intestazione_style brand_color_txt">our buiseness areas</h5>
            <h1 class="title_style">Exellence in <div class="underline_title brand_color_base brand_color_txt">Services</div></h1>
            <!-- Contenuto sottotitolo + bottone -->
            <div class="d-flex justify-content-between align-items-center color_gray_txt my-4">
                <p class="w-75">
                    We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.
                </p>
                <div class="button_style">see all</div>
            </div>
            <!-- Stampa card -->
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