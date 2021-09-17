<template>
  <!-- Template della singola card utilizzata in Menagement.vue -->
  <div class="management_card d-inline-block position-relative align-top">
    <!-- Intestazione della card contenente il numero di index dell'item, aumentato di uno e formattato in modo che mostri due cifre significative -->
    <div class="d-inline-block position-absolute top-0 start-50 translate-middle rounded-style brand_color_lighter brand_color_txt fw-bold">{{ String(this.itemIndex+1).padStart(2, '0') }}</div>
    
    <!-- Ttitolo della card + contenuto (rucevuti via props)-->
    <h4 class="fw-bold mb-3 mt-5 mx-3"> {{item.title}} </h4>
    <p class="color_gray_txt"> {{item.text}} </p>
  </div>
</template>

<script>
export default {
  name: 'ManagementCard',
  props: ['item', 'itemIndex'],
}
</script>

<style>
.management_card {
    width: 20%;
}
</style>