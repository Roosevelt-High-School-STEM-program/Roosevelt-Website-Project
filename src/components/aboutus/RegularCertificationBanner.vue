<template>
  <div
    class="row"
    style="
      height: 205px;
      background-image: url('../../statics/food-pictures/oatMeatSpreadOut.JPG');
      background-size:cover;"
  >
    <div
      class="row justify-center items-center col-md-12"
      style="background-color: rgba(20, 15, 15, 0.6);"
    >
      <div
        class="row justify-center col-md-4 text-center"
        style="letter-spacing: 2px;"
      >
        <p
          class="text-weight-bold text-white no-hightlight"
          style="font-size: 33px;
            font-family: Alegreya Sans SC;
            text-align: center;"
        >
          Here at Honolulu
          <br>
          Baking Company, We are
        </p>
      </div>
      <div class="col-md-1" />
      <div class="col-md-3">
        <q-img
          style="max-width: 120px;"
          src="../../statics/cert/USDA&FDAWhite.png"
        />
      </div>
      <div class="col-md-3">
        <q-img
          style="max-width: 270px;"
          src="../../statics/cert/Military&state&SQF2White.png"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CertificationBanner',
};
</script>

<style scoped>

</style>
