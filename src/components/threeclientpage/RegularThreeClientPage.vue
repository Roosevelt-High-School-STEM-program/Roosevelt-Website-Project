<template>
  <div class="col-md-12 row" style="height:800px;">
    <div
      class="col-md-4 row justify-center"
    >
      <q-img v-ripple src="../../statics/hand-cut.jpeg">
        <div
          class="row items-center justify-center button-properties text-weight-bold img-styling"
        >
          HAND-CUT PRODUCE
        </div>
      </q-img>
    </div>
    <div class="col-md-4 row justify-center">
      <q-img v-ripple src="../../statics/scones.jpeg">
        <div
          class="row items-center justify-center button-properties text-weight-bold img-styling"
        >
          BAKERY
        </div>
      </q-img>
    </div>
    <div class="col-md-4 row justify-center">
      <q-img v-ripple src="../../statics/scones.jpeg">
        <div
          class="row items-center justify-center button-properties text-weight-bold img-styling"
        >
          Bakery
        </div>
      </q-img>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ThreeClientPage',
};
</script>

<style scoped lang="scss">
  .button-properties {
    cursor: pointer;
    transition: all .27s linear;
  }
  .button-properties:hover {
    background-color: rgba(0, 0, 0, 0.5);
    transition: all .27s linear;
  }
  #hand-cut-produce {
    background-size: cover;
  }
  #bakery {
    background-size: cover;
  }
  /*TODO change the name of this variable to match whatever the client wanted*/
  #changeNameLater {
    background-image: url("../../statics/salads.jpeg");
    background-size: cover;
  }
  .img-styling {
    width: 100%;
    height:100%;
    font-size:32px;
    font-family: Alegreya Sans SC;
    letter-spacing: 3px;
    color: $website-light-brown;
  }
</style>
