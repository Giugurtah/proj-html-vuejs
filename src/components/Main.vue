<template>
    <main>
        <Jumbotron />
        <Company />
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Company from "./Company.vue"
export default {
  name: "Main",
  components: {
      Jumbotron,
      Company,
  }
}
</script>

<style>

</style>