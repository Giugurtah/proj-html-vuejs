<template>
    <section id="List" class="aux_color_darker p-standard"> 
        <div class="container aux_color_light_txt">
            <div class="row gx-5">
                <div class="col-3">
                    <Logo :colorText="'color_white_txt'"/>
                    <p class="my-4">
                        A Functional HTML Template for Corporate & Business.
                    </p>
                    <div class="my-1">
                        <i class="fas fa-phone-alt me-3"></i>
                        +1(305)1234-5678
                    </div>
                    <div class="my-1">
                        <i class="fas fa-envelope me-3"></i>
                        hello@xexample.com
                    </div>
                    <div class="my-1">
                        <i class="fas fa-map-marker-alt me-3"></i>
                        Main Avenue, 987
                    </div>
                    <div class="button_style button_alternative color_white_txt mt-5">get in touch</div>
                </div>
                <ListCard v-for="(item, index) in listData" :key="index" :item="item" />
            </div>
        </div>
    </section>
</template>

<script>
import Logo from "../Logo.vue";
import listData from "../../assets/data/list.js";
import ListCard from "./ListCard.vue";
export default {
  name: 'List',
  components: {
    Logo,
    ListCard,
  },
  data() {
    return {
        listData
    }
  }
}
</script>

<style>

</style>