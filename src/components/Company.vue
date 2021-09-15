<template>
  <div id="company" class="d-flex align-items-center aux_color_darker">
      <div class="container">
          <h6 class="uppercase brand_color_txt fw-bold">About the network</h6>
          <div class="row aux_color_light_txt">
              <div class="col-6 pe-5">
                  <h1 class="color_white_txt"><div class="d-inline-block aux_color_dark">The</div> Company</h1>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt quod nisi beatae minima dolorem alias expedita maxime quisquam quis. Minus aperiam nihil placeat nulla</p>
                  <p class="mt-1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus vitae voluptatum quo labore officia nihil consequuntur</p>
              </div>
              <div class="col-6">
                  <div class="row">
                      <div class="col-6" v-for="(item, index) in company" :key="index">
                          <h4 class="my-3 color_white_txt"><i :class="item.icon" class="fas brand_color_txt me-1"></i> {{item.title}}</h4>
                          <p>{{item.text}}</p>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
import company from "../assets/data/company.js"
export default {
  name: 'Company',
  data() {
      return {
          company,
      }
  }
}
</script>

<style>
#company {
    height: 450px;
}
</style>