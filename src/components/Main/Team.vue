<template>
    <!-- Section contenenti le info del team aziendale -->
    <section id="team" class="team aux_color_darker p-standard">
        <div class="container">
            <div class="row">
                <div class="col-8">
                    <!-- Titolo + intestazione -->
                    <h6 class="intestazione_style brand_color_txt">we like what to do</h6>
                    <h1 class="title_style color_white_txt"><div class="underline_title aux_color_dark">Team</div> of experts</h1>
                    <!-- Contenuto sottotitolo -->
                    <p class="aux_color_light_txt my-4">
                    Ethics and integrity are the bases on which our professionals build their careers.
                    <br>
                    They are fundamentals that become daily attitudes.
                    </p>
                    <!-- Stampa card -->
                    <div class="row">
                        <TeamCard v-for="(item, index) in teamData" :key="index" :item="item" />
                    </div>
                </div>
                <!-- Contenuto informativo -->
                <div class="col-4 position-relative brand_color aux_color_light_txt rounded-2 mt-4 p-5">
                    <!-- Titolo -->
                    <h6 class="fw-bold color_white_txt">President Speach</h6>
                    <!-- Contenuto -->
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ut lacinia diam</p>
                    <p>Vivamus efficitur et est quis posuere. Nulla sollicitudin vulputate dui, id pretium tortor congue eu. Integer aliquet justo eu quam volutpat ullamcorper.</p>
                    <p>Duis ut hendrerit mauris. Phasellus faucibus enim vel tincidunt Nunc venenatis a dui et laoreet.</p>
                    <!-- Citazione -->
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