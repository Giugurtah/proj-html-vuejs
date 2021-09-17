<template>
  <!-- Section contentente le info sulla compagnia -->
  <section id="company" class="aux_color_darker p-standard">
      <div class="container">
          <div class="row aux_color_light_txt">
              <div class="col-6 pe-5">
                  <!-- Titolo + intestazione -->
                  <h5 class="intestazione_style brand_color_txt">About the network</h5>
                  <h1 class="title_style color_white_txt"><div class="underline_title aux_color_dark">The</div> Company</h1>
                  <!-- Contenuto sotto titolo -->
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt quod nisi beatae minima dolorem alias expedita maxime quisquam quis. Minus aperiam nihil placeat nulla</p>
                  <p class="mt-1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus vitae voluptatum quo labore officia nihil consequuntur</p>
              </div>
              
              <div class="col-6">
                  <div class="row">
                      <!-- Stampa contenuti di companyData -->
                      <div class="col-6 my-2" v-for="(item, index) in companyData" :key="index">
                          <h4 class="mb-3 color_white_txt"><i :class="item.icon" class="fas brand_color_txt me-1"></i> {{item.title}}</h4>
                          <p>{{item.text}}</p>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
import companyData from "../../assets/data/company.js"
export default {
  name: 'Company',
  data() {
      return {
          companyData,
      }
  }
}
</script>

<style>
</style>