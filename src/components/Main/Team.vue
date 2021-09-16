<template>
  <section id="team" class="team aux_color_darker p-standard">
      <div class="container">
          <h6 class="uppercase brand_color_txt fw-bold">we like what to do</h6>
            <div class="row">
                <div class="col-8">
                    <h1 class="color_white_txt"><div class="d-inline-block aux_color_dark px-2">Team</div> of experts</h1>
                    <p class="aux_color_light_txt my-4">
                    Ethics and integrity are the bases on which our professionals build their careers.
                    <br>
                    They are fundamentals that become daily attitudes.
                    </p>
                    <div class="row">
                        <TeamCard v-for="(item, index) in teamData" :key="index" :item="item" />
                    </div>
                </div>
                <div class="col-4 position-relative brand_color aux_color_light_txt rounded-2 p-5">
                    <h6 class="fw-bold color_white_txt">President Speach</h6>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ut lacinia diam</p>
                    <p>Vivamus efficitur et est quis posuere. Nulla sollicitudin vulputate dui, id pretium tortor congue eu. Integer aliquet justo eu quam volutpat ullamcorper.</p>
                    <p>Duis ut hendrerit mauris. Phasellus faucibus enim vel tincidunt Nunc venenatis a dui et laoreet.</p>
                    <h6 class="fw-bold color_white_txt">T.Johnson</h6>

                    <i class="fas fa-quote-right position-absolute end-0 bottom-0 aux_color_dark_txt fs-2 p-5"></i>
                </div>
            </div>
      </div>
  </section>
</template>

<script>
import teamData from "../../assets/data/team";
import TeamCard from "./TeamCard.vue";
export default {
  name: 'Team',
  components: {
      TeamCard,
  },
  data() {
      return {
          teamData,
      }
  }
}
</script>

<style>

</style>