<template>
  <!-- Section contenete le info di contatto del cliente -->
  <section id="contacts" class="aux_color_dark aux_color_lighter_txt">
    <div class="container d-flex justify-content-between p-2 fs-6">
      <!-- Info a sx contenete gli orari di apertura -->
      <div>
        <i class="fas fa-clock"></i>
        Open Haurs: Mon - Sat - 9:00 - 18:00
      </div>
      <!-- Info a dx contenet i recapiti -->
      <div>
        <div class="d-inline-block mx-3">
          <i class="fas fa-phone-alt"></i>
          +1(305)1234-5678
        </div>
        <div class="d-inline-block mx-3">
          <i class="fas fa-envelope"></i>
          hello@xexample.com
        </div>
        <div class="d-inline-block mx-3">
          <i class="fab fa-facebook-f me-3"></i>
          <i class="fab fa-twitter mx-3"></i>
          <i class="fab fa-linkedin-in ms-3"></i>
        </div>
      </div>
    </div>      
  </section>
</template>

<script>
export default {
  name: 'Contacts',
}
</script>

<style scoped>
</style>