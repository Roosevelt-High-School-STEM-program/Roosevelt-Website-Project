<template>
  <div
    class="row justify-center items-center bg-white"
    style="min-height:520px"
  >
    <div class="col-md-1 col-xs-8 q-mt-none" />
    <div class="col-md-4 col-xs-11 text-center">
      <h1
        class="q-my-none text-weight-bold"
        style="font-size: 45px; letter-spacing: 2px;"
      >
        Our Story
      </h1>
      <p
        :class="$q.screen.sm || $q.screen.lt.sm ? 'anaheim' : 'anaheim q-mt-sm'"
        :style="$q.screen.lt.sm ? 'font-size:17px;' : 'font-size:19px;'"
      >
        It is a long established fact that a reader will be distracted by
        the readable content of a page when looking at its layout. The point of using Lorem I
        psum is that it has a more-or-less normal distribution of letters, as opposed to using
        'Content here, content here', making it look like readable English.
      </p>
    </div>
    <div class="col-md-2" />
    <div
      :class="$q.screen.sm || $q.screen.lt.sm ?
        'row justify-center col-xs-8 col-sm-12 order-first q-mt-lg' : 'col-md-2 '"
    >
      <q-img
        class="float-image"
        :style="$q.screen.sm || $q.screen.lt.sm ? 'max-width:280px' : 'max-width:320px'"
        src="../../statics/food-pictures/oatCakeTopDown.png"
      />
    </div>
    <div class="col-md-2"/>
  </div>
</template>

<script>

export default {
  name: 'AboutUs',
};
</script>

<style scoped>
  h1 {
    font-family: Alegreya Sans SC, cursive;
  }
</style>
