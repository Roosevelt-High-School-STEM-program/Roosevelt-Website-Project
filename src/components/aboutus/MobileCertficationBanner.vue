<template>
    <q-carousel
      style="height: 205px;"
      class="col-xs-4"
      animated
      v-model="slide"
      autoplay="true"
      arrows
      infinite
    >
      <q-carousel-slide
        :name="1"
        class="padding-none"
        img-src="../../statics/food-pictures/oatMeatSpreadOut.jpg"
      >
        <div class="text-center grey-overlay">
          <p class="text-weight-bold text-white no-hightlight padding-none">
            Here at Honolulu
            <br>
            Baking Company,
            <br>
            We are ...
          </p>
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        :name="2"
        class="padding-none"
        img-src="../../statics/food-pictures/oatMeatSpreadOut.jpg"
      >
        <div class="text-center grey-overlay">
          <q-img
            style="max-width: 270px;"
            src="../../statics/cert/Military&state&SQF2White.png"
          />
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        :name="3"
        class="padding-none"
        img-src="../../statics/food-pictures/oatMeatSpreadOut.jpg"
      >
        <div class="text-center grey-overlay">
          <q-img
            style="max-width: 130px;"
            src="../../statics/cert/USDA&FDAWhite.png"
          />
        </div>
      </q-carousel-slide>
    </q-carousel>
</template>

<script>
export default {
  name: 'MobileCertificationBanner',
  data() {
    return {
      slide: 1,
    };
  },
};
</script>

<style scoped>
  .padding-none {
    padding: 0 0 0 0;
  }
  .grey-overlay {
    height: 100%;
    width:100%;
    background-color: rgba(20, 15, 15, 0.6);
    padding:16px;
  }
  p {
    font-size: 37px;
    font-family: Alegreya Sans SC;
    text-align: center;
  }
</style>
