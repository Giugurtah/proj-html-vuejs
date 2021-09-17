<template>
    <!-- Main del sito -->
    <main>
        <Jumbotron />
        <Company />
        <Services />
        <Management />
        <Team />
        <News />
        <Newsletter />
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Company from "./Company.vue";
import Services from "./Services.vue";
import Management from "./Management.vue";
import Team from "./Team.vue";
import News from "./News.vue";
import Newsletter from "./Newsletter.vue";
export default {
  name: "Main",
  components: {
      Jumbotron,
      Company,
      Services,
      Management,
      Team,
      News,
      Newsletter
  }
}
</script>

<style>

</style>