<template>
  <div class="row">
    <div class="col-md-12 column" style="height:720px">
      <div
        class="col-md-12 row"
        id="front-page-image"
      >
        <div
          class="col-md-12 row items-center justify-center"
          style="background-color: rgba(0, 0, 0, 0.6);"
        >
          <div class="col-md-5 no-hightlight text-white text-center" >
            <h1>Honolulu Baking Company</h1>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RegularOpeningScreen',
};
</script>

<style scoped>
  #front-page-image {
    background-image: url('/statics/food-pictures/oatCake.JPG');
    background-position: center;
    background-size: cover;
    min-height: 100%;
  }
  h1 {
    font-family: Alegreya Sans SC;
    letter-spacing: 2px;
  }
</style>
