<template>
  <div
    class="row justify-center items-center bg-white"
    style="min-height:520px"
  >
    <div class="col-md-1 col-xs-8 q-mt-none" />
    <div
      class="col-md-4 col-xs-11 text-center"
      style="font-family: Alegreya Sans SC, cursive;"
    >
      <h1
        class="q-my-none text-weight-bold"
        style="font-size: 45px; letter-spacing: 2px"
      >
        About Us
      </h1>
      <p
        :class="$q.screen.sm || $q.screen.lt.sm
          ?'' : 'q-mt-sm'"
        :style="$q.screen.sm || $q.screen.lt.sm
        ? 'font-size:17px; font-family: Anaheim' : 'font-size:19px; font-family: Anaheim'"
      >
        It is a long established fact that a reader will be distracted by
        the readable content of a page when looking at its layout. The point of using Lorem I
        psum is that it has a more-or-less normal distribution of letters, as opposed to using
        'Content here, content here', making it look like readable English.
      </p>
    </div>
    <div class="col-md-2" />
    <div :class="$q.screen.sm || $q.screen.lt.sm ?
     'row col-md-4 col-xs-8 order-first q-mt-lg' : 'row col-md-4 col-xs-10'"
    >
      <q-img
        class="float-image"
        style="max-width:320px"
        src="../../statics/food-pictures/oatCakeTopDown.png"
      />
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
