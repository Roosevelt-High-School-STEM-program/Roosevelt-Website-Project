<template>
  <div class="row bg-website-white" style="min-height:800px;">
      <div
        class="row justify-center items-center"
        style="height:513px"
      >
        <div class="col-md-1 q-mt-none" />
          <div
            class="col-md-4 text-center"
            style=" font-family: Alegreya Sans SC, cursive;"
          >
            <h1
              class="q-my-none text-weight-bold letter-spacing: 3px;"
              style="font-size: 45px"
            >
              welcome
            </h1>
            <p class="q-mt-sm" style="font-size:19px; font-family: 'Anaheim'">
              It is a long established fact that a reader will be distracted by
              the readable content of a page when looking at its layout. The point of using Lorem I
              psum is that it has a more-or-less normal distribution of letters, as opposed to using
              'Content here, content here', making it look like r
              eadable English. Many desktop publishing packages and web pa
              ge editors now use Lorem Ipsum as their default model text,
              and a search for 'lorem ipsum' will uncover many web sites stil
              l in their infancy. Various versions have evolved over the years,
              sometimes by accident, sometimes on purpose (injected humour and
              the like).
            </p>
          </div>
          <div class="col-md-2" />
          <div class="row col-md-4">
            <q-img
              class="float-image"
              style="max-width:320px"
              src="../../statics/food-pictures/oatCakeTopDown.png"
            />
        </div>
      </div>
    <div
      class="row col-md-12"
      style="
      background-image: url('../../statics/food-pictures/oatMeatSpreadOut.JPG');
      background-size:cover;
      background-color: rgba(0, 0, 0, 0.6);"
    >
      <div
        class="row justify-center items-center col-md-12"
        style="background-color: rgba(56, 41, 19, 0.6);"
      >
      <div
        class="row justify-center col-md-4 text-center"
        style="letter-spacing: 2px;"
      >
          <p
            class="text-weight-bold text-website-page-cutter-red"
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
          src="../../statics/cert/USDA&FDA.png"
        />
      </div>
      <div class="col-md-3">
        <q-img
          style="max-width: 270px;"
          src="../../statics/cert/Military&state&SQF2.png"
        />
      </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'RegularAbout',
};
</script>

<style scoped>

</style>
