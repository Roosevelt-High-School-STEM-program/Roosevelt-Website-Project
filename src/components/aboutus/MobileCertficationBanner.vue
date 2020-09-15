<template>
    <q-carousel
      style="height: 205px; "
      class="col-xs-4"
      animated
      v-model="slide"
      autoplay="true"
      arrows
      infinite
    >
      <q-carousel-slide
        :name="1"
        img-src="../../statics/food-pictures/oatMeatSpreadOut.jpg"
        style="padding:0 0 0 0;"
      >
        <div
          class="text-center"
          style="
          height: 100%;
          width:100%;
          background-color: rgba(20, 15, 15, 0.6);
          padding:16px"
        >
          <p
            class="text-weight-bold text-white no-hightlight"
            style="font-size: 37px;
              font-family: Alegreya Sans SC;
              text-align: center;"
          >
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
        img-src="../../statics/food-pictures/oatMeatSpreadOut.jpg"
        style="padding:0 0 0 0;"
      >
        <div
          class="text-center"
          style="
          height: 100%;
          width:100%;
          background-color: rgba(20, 15, 15, 0.6);
          padding:16px"
        >
          <q-img
            style="max-width: 270px;"
            src="../../statics/cert/Military&state&SQF2White.png"
          />
        </div>

      </q-carousel-slide>
      <q-carousel-slide
        :name="3"
        class="text-center"
        img-src="../../statics/food-pictures/oatMeatSpreadOut.jpg"
        style="padding:0 0 0 0;"
      >
        <div
          class="text-center"
          style="
          height: 100%;
          width:100%;
          background-color: rgba(20, 15, 15, 0.6);
          padding:16px"
        >
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
  name: 'MobileCertficationBanner',
  data() {
    return {
      slide: 1,
    };
  },
};
</script>

<style scoped>

</style>
