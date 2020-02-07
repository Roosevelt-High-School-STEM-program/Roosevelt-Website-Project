<template>
  <div class="row">
    <div class="col-md-12 column" style="height:710px">
      <!-- Note is that the box is not resizing because
       the background is taking up 100% of the page -->
      <div
        class="col-md-12 row"
        style="
        background-image: url('../../statics/oatMealCake.jpg');
        background-size: 100%;
        min-height:100%;
        font-family: Satisfy, cursive;
        "
      >
        <div
          class="col-md-12 row justify-center"
          style="background-color: rgba(255,255,255,0.3)"
        >
          <div class="col-md-4 q-mt-lg">
            <q-img src="../../statics/HonoluluBakingCircle.png"/>
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

</style>
