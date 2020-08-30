<template>
  <div class="row text-white background-img">
    <div
      class="row col-md-12 justify-center q-my-none bg-website-white"
      style="height: 325px; background-color: rgba(20, 15, 15, 0.7);"
    >
      <div class="col-md-12 row justify-center text-center">
        <div class="col-md-12" />
        <div class="col-md-12 q-my-none">
          <h1 class="q-my-sm text-weight-medium no-hightlight">
            CONTACT INFO
          </h1>
        </div>
        <div class="col-md-8 col-lg-7 row">
          <div class="col-md-4">
            <div class="row justify-center items-center">
              <q-icon name="place" size="20px" />
              <p class="q-ma-sm text-weight-bold contact-info no-hightlight">
                Address
              </p>
            </div>
            <p class="q-ma-sm text-weight-medium" style="font-size:17px">
              523 Ahui St, Honolulu, HI 96813
            </p>
          </div>
          <div class="col-md-4">
            <div class="row justify-center items-center">
              <q-icon name="phone" size="20px" />
              <p class="q-ma-sm text-weight-bold contact-info no-hightlight">Phone</p>
            </div>
            <p class="q-ma-sm text-weight-medium" style="font-size: 17px">
              (808) 596-8415
            </p>
          </div>
          <div class="col-md-4">
            <div class="row justify-center items-center">
              <q-icon name="img:../../statics/instagramGlyphLogo.png" size="18px" />
              <p class="q-ma-sm text-weight-bold contact-info no-hightlight">Instagram</p>
            </div>
            <p class="q-ma-sm text-weight-medium" style="font-size:17px">
              @OriginalHawaiiOatCake
            </p>
          </div>
        </div>
        <div class="col-md-12" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RegularContactUs',
};
</script>

<style scoped>
 .contact-info {
   font-size:19px;
   letter-spacing: 2px
 }
  .background-img {
    background-image: url('../../statics/food-pictures/oatmeal.jpg');
    background-size:cover;
  }
  h1 {
    font-family: Alegreya Sans SC;
    letter-spacing: 2px;
    font-size:90px
  }
</style>
