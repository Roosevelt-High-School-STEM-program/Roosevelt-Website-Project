<template>
  <div class="col-md-12 row">
    <q-list class="col-12 row text-weight-bold">
      <q-item
        class="col-4 q-pa-none"
        clickable
        v-ripple
        style="background-image: url('../../statics/hand-cut.jpeg'); background-size: cover;"
        to="hand-cut-produce"
      >
        <div class="column justify-center image-cover">
          <q-item-section class="text-center col image-text">
            HAND-CUT PRODUCE
          </q-item-section>
        </div>
      </q-item>
      <q-item
        class="col-4 q-pa-none"
        clickable
        v-ripple
        style="background-image: url('../../statics/scones.jpeg'); background-size: cover;"
      >
        <div class="column justify-center image-cover">
          <q-item-section class="text-center col image-text">
            BAKERY
          </q-item-section>
        </div>
      </q-item>
      <q-item
        class="col-4 q-pa-none"
        clickable
        v-ripple
        style="background-image: url('../../statics/scones.jpeg'); background-size: cover;"
      >
        <div class="column justify-center image-cover">
          <q-item-section class="text-center col image-text">
            BAKERY
          </q-item-section>
        </div>
      </q-item>
    </q-list>
  </div>
</template>

<script>
export default {
  name: 'ThreeClientPage',
  // TODO May remove this page due to it being irrelevant dk yet
};
</script>

<style scoped type="text/scss" lang="scss">
  /*.button-properties {*/
  /*  cursor: pointer;*/
  /*  transition: all .27s linear;*/
  /*}*/
  /*.button-properties:hover {*/
  /*  background-color: rgba(0, 0, 0, 0.5);*/
  /*  transition: all .27s linear;*/
  /*}*/
  /*#hand-cut-produce {*/
  /*  background-size: cover;*/
  /*}*/
  /*#bakery {*/
  /*  background-size: cover;*/
  /*}*/
  /*TODO change the name of this variable to match whatever the client wanted*/
  /*#changeNameLater {*/
  /*  background-image: url("../../statics/salads.jpeg");*/
  /*  background-size: cover;*/
  /*}*/
  .img-styling {
    width: 100%;
    height:100%;
    font-size:32px;
    font-family: Alegreya Sans SC;
    letter-spacing: 3px;
    color: $website-light-brown;
  }
  .image-cover {
    width:100%;
    height:100%;
    background-color: rgba(0, 0, 0, 0.5);
  }
  .image-text {
    font-size:32px;
    color: $website-red;
    letter-spacing: 3px;
    user-select: none;
  }
</style>
