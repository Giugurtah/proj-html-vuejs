<template>
  <section id="jumbotron" class="position-relative">
      <form >
        <h5 class="uppercase brand_color_light_txt">fusion & aquisitions</h5>
        <h1>Insurance Consulting</h1>
        <div class="row g-1">
            <div class="col-6 pe-2 py-2"><input class="w-100 form_style" type="text" placeholder="Name" name="" id=""></div>
            <div class="col-6 py-2"><input class="w-100 form_style" type="email" placeholder="Email" name="" id=""></div>
            <div class="col-6 pe-2 py-2"><input class="w-100 form_style" type="tel" placeholder="Phone" name="" id=""></div>
            <div class="col-6 py-2">
                <select class="w-100 form_style h-100" name="" id="">
                    <option default value="More info">More info</option>
                    <option  value="Name">Name</option>
                    <option  value="Email">Email</option>
                    <option  value="Phone">Phone</option>
                </select>
            </div>
        </div>
        <div class="buttons py-2">
            <div class="button_style me-3">get in touch</div>
            <div class="button_style button_alternative">read more</div>
        </div>
      </form>
  </section>
</template>

<script>
export default {
  name: "Jumbotron",
}
</script>

<style lang="scss">
@import "../../assets/style/_variables.scss";
#jumbotron {
    background-image: url("../../assets/img/bg-6.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position-y: -20px ;
    background-position-x: left;
    height: 600px;

    position: relative;

    ::placeholder {
        color: $gray_shade;
        opacity: 1;
    }

    form {
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translateY(-50%);
        width: 550px;
    }
}
// Overlay usato per regolare la tonalità dello sfondo del jumbotron con il nuovo tema
#jumbotron:before {
        content: "";
        position: absolute;
        left: 0; right: 0;
        top: 0; bottom: 0;
        background: rgba(231,130,130,.1);
    }
</style>