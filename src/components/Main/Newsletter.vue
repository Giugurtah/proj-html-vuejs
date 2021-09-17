<template>
  <!-- Section che contiene un form per iscriversi alla newsletter -->
  <section id="newsletter" class="p-standard">
      <div class="w-75 mx-auto">
          <div class="row">
              <div class="col-6">
                <!-- Titolo + intestazione -->
                <h6 class="intestazione_style brand_color_txt">Newsletter</h6>
                <h1 class="title_style color_white_txt"><div class="underline_title aux_color_dark">Know</div> First</h1>
                <!-- Contenuto sottotitolo -->
                <p class="aux_color_light_txt my-4">
                Follow closely and receive content about our company and the news of the current market.
                </p>
              </div>
              <!-- Form -->
              <form class="col-6 my-auto ps-3">
                <!-- Nome -->
                <input class="w-75 my-2 form_style" type="text" placeholder="Name" name="" id="">
                <!-- Email -->
                <input class="d-block w-75 my-2 form_style" type="email" placeholder="Email" name="" id="">
                <!-- Bottone -->
                <div class="button_style my-2">subscribe</div>
              </form>
          </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss">
// Style custom del background della section
#newsletter {
    background-image: url("../../assets/img/bg-1.jpg");
    background-position: center;
    background-size: cover;
}
</style>