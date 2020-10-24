<template>
  <div class="row">
    <div class="col-md-12 col-sm-12 col-xs column" style="height:95vh">
      <div
        class="col-md-12 col-sm-12 col-xs row"
        id="front-page-image"
      >
        <div
          class="col-md-12 col-sm-12 col-xs row items-center justify-center"
          style="background-color: rgba(0, 0, 0, 0.6);"
        >
          <div class="col-md-5 col-sm-7 col-xs no-hightlight text-white text-center" >
            <h1 :style="$q.screen.lt.sm ? 'font-size:70px' : ''">Honolulu Baking Company</h1>
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
    background-image: url('../../statics/food-pictures/oatCake.jpg');
    background-position: center;
    background-size: cover;
    min-height: 100%;
  }
  h1 {
    font-family: Alegreya Sans SC;
    letter-spacing: 2px;
  }
</style>
