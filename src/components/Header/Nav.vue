<template>
  <!-- Section contenente la barra di navigazione interna del sito -->
  <section id="nav" class="container d-flex justify-content-between align-content-center py-2">
      <!-- Componenete logo del clienete -->
      <Logo :colorText="''" />
      <div class="my-2">
        <!-- Barra di navigazione interna -->
        <ul>
          <!-- Stampa singoli link presenti in dataNav -->
          <li v-for="(data, index) in navData" :key="index" class="uppercase color_gray_txt mx-3"> 
              <a href="#"> {{data}} </a>
          </li>
        </ul>
        <button class="button_style">Get in touch</button>
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

<style>
</style>