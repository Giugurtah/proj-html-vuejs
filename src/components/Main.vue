<template>
    <main>
        <Jumbotron />
        <Company />
        <Services />
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Company from "./Company.vue";
import Services from "./Services.vue"
export default {
  name: "Main",
  components: {
      Jumbotron,
      Company,
      Services,
  }
}
</script>

<style>

</style>