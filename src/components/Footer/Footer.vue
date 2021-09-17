<template>
    <footer>
        <List :colorText="'color_white_txt'" /> 
        <PoweredBy />
    </footer>
</template>

<script>
import List from "./List.vue";
import PoweredBy from "./PoweredBy.vue";
export default {
  name: "Footer",
  components: {
      List,
      PoweredBy,
  }
}
</script>

<style>

</style>