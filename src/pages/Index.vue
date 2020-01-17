<template>
  <q-page class="row">
    <div class="col-md-12 column" style="height:710px">
      <!-- Note is that the box is not resizing because
       the background is taking up 100% of the page -->
      <div
        class="col-md-12 row"
        style="
        background-image: url('../statics/oatMealCake.jpg');
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
            <img class="col-4" src="../statics/HonoluluBakingCircle.png"/>
          </div>
        </div>
      </div>
    </div>
    <div class="col-md-12 row" style="background-color: #FFD046">
      <div
        class="col-md-6"
        style="background-image: url('../statics/pastry.jpg'); background-size:100%"
      >
      </div>
      <div class="col-md-6">
        <h1>
          Incredibly Inspiring words Incredibly Inspiring words
        </h1>
        <p>
          Incredibly Inspiring words Incredibly Inspiring words
        </p>
    </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
};
</script>
