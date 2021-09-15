<template>
  <div id="jumbotron" >
      <form >
        <h5 class="uppercase brand_color_light_txt">fusion & aquisitions</h5>
        <h1>Insurance Consulting</h1>
        <div class="row g-1">
            <div class="col-6 p-2"><input class="w-100 form_style" type="text" placeholder="Name" name="" id=""></div>
            <div class="col-6 p-2"><input class="w-100 form_style" type="email" placeholder="Email" name="" id=""></div>
            <div class="col-6 p-2"><input class="w-100 form_style" type="tel" placeholder="Phone" name="" id=""></div>
            <div class="col-6 p-2">
                <select class="w-100 form_style h-100" name="" id="">
                    <option default value="More info">More info</option>
                    <option  value="Name">Name</option>
                    <option  value="Email">Email</option>
                    <option  value="Phone">Phone</option>
                </select>
            </div>
        </div>
      </form>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
}
</script>

<style lang="scss">
@import "../assets/style/_variables.scss";
#jumbotron {
    background-image: url("../assets/img/bg-6.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position-y: -20px ;
    background-position-x: left;
    height: 600px;

    position: relative;

    ::placeholder {
        color: $aux_color_light;
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
</style>