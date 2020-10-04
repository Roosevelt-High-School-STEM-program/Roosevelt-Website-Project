<template>
  <div class="row justify-center items-center col-md-12 col-xs-12 q-my-md bg-white q-mb-lg">
    <div class="col-md-3 col-xs-1" />
    <div class="col-md-3 col-xs-8 col-sm-6 q-mt-md">
      <q-img src="../../statics/Ohana2.png" />
    </div>
    <div class="col-md-3 col-xs-1" />
    <div class="col-md-6 col-xs-11 q-mt-lg">
      <q-img
        class="float-image"
        style="background-position: center;"
        :ratio="870/480"
        src="../../statics/people-photos/groupPic.jpeg"
      />
    </div>
    <div class="col-md-4 offset-md-1 col-xs-11 text-center">
      <h1
        class="q-my-none text-weight-bold"
        style="font-size: 45px; letter-spacing: 2px;"
      >
        Family
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

<!--    <div class="col-md-12 q-mt-lg" />-->
  </div>

</template>

<script>
export default {
  name: 'OurOhana',
};
</script>

<style scoped>
  h1 {
    font-family: Alegreya Sans SC, cursive;
  }
</style>
