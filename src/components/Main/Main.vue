<template>
    <main>
        <Jumbotron />
        <Company />
        <Services />
        <Management />
        <Team />
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Company from "./Company.vue";
import Services from "./Services.vue";
import Management from "./Management.vue";
import Team from "./Team.vue";
export default {
  name: "Main",
  components: {
      Jumbotron,
      Company,
      Services,
      Management,
      Team,
  }
}
</script>

<style>

</style>